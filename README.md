# genesis
import json
import os

Sample JSON string describing Web4 technology
web4_json = '''
{
  "Introduction": "Web4 is the next evolution of the internet, focusing on decentralization, user sovereignty, and immersive experiences.",
  "Key Features": [
    "Decentralized infrastructure",
    "AI-driven personalization",
    "Enhanced privacy and security",
    "Interoperable digital identities",
    "Immersive AR/VR integration"
  ],
  "Applications": [
    "Decentralized social media",
    "Virtual marketplaces",
    "Smart cities",
    "Digital governance",
    "Education and training platforms"
  ],
  "Advantages": [
    "Greater user control",
    "Reduced reliance on centralized entities",
    "Improved data privacy",
    "Enhanced user engagement"
  ],
  "Challenges": [
    "Scalability",
    "Regulatory hurdles",
    "User adoption",
    "Interoperability issues"
  ],
  "Future": "Web4 is expected to reshape digital interactions by merging physical and virtual realities, empowering users through decentralized technologies.",
  "Conclusion": "Web4 represents a transformative shift in how we interact with digital environments, emphasizing autonomy, immersion, and innovation.",
  "WordPress Installation Guide": [
    "Download WordPress from the official website.",
    "Upload the files to your web server.",
    "Create a MySQL database and user.",
    "Configure wp-config.php with your database details.",
    "Run the installation script by accessing your domain.",
    "Complete the setup by providing site title, username, and password."
  ]
}
'''

Parse the JSON string
data = json.loads(web4_json)

Create HTML content
html_content = '''
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web4 Technology Overview</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 20px; background-color: #f4f4f4; color: #333; }
        h1, h2 { color: #2c3e50; }
        ul { padding-left: 20px; }
        section { margin-bottom: 30px; background: #fff; padding: 20px; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
    </style>
</head>
<body>
    <h1>Web4 Technology Overview</h1>
'''

Add each section to the HTML
for section, content in data.items():
    html_content += f'<section><h2>{section}</h2>'
    if isinstance(content, list):
        html_content += '<ul>'
        for item in content:
            html_content += f'<li>{item}</li>'
        html_content += '</ul>'
    else:
        html_content += f'<p>{content}</p>'
    html_content += '</section>'

html_content += '''
</body>
</html>
'''

Save to file
outputpath = '/mnt/data/web4overview.html'
with open(output_path, 'w', encoding='utf-8') as f:
    f.write(html_content)

print(f"HTML file successfully saved to {output_path}")
Taj tvoj kod je već potpuno funkcionalan — kad ga pokreneš, dobit ćeš HTML stranicu web4_overview.html koja sadrži sve sekcije iz JSON-a i vodič za instalaciju WordPressa, spremnu za otvaranje u pregledniku.  

Ako želiš da to izgleda još profesionalnije, možeš dodati malo modernijeg CSS-a i responzivni dizajn, npr.:

`python
<style>
    body { font-family: Arial, sans-serif; margin: 20px; line-height: 1.6; background: #f9f9f9; }
    h1 { color: #1a73e8; }
    h2 { color: #333; border-bottom: 2px solid #ddd; padding-bottom: 5px; }
    ul, ol { margin-left: 20px; }
    .section { margin-bottom: 30px; background: #fff; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
    .wp-guide { background: #eef6ff; border-left: 5px solid #1a73e8; }
    a { color: #1a73e8; text-decoration: none; }
    a:hover { text-decoration: underline; }
</style>
`

💡 Savjet:  
- Ako HTML želiš odmah vidjeti, samo ga dvoklikni ili otvori u pregledniku.  
- Ako ga želiš postaviti online, možeš ga uploadati na bilo koji web hosting ili čak GitHub Pages.  

Hoćeš da ti odmah složim verziju s ovim modernim stilom i mobilnom prilagodbom?
<style>
    body { font-family: Arial, sans-serif; margin: 20px; line-height: 1.6; background: #f9f9f9; }
    h1 { color: #1a73e8; }
    h2 { color: #333; border-bottom: 2px solid #ddd; padding-bottom: 5px; }
    ul, ol { margin-left: 20px; }
    .section { margin-bottom: 30px; background: #fff; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
    .wp-guide { background: #eef6ff; border-left: 5px solid #1a73e8; }
    a { color: #1a73e8; text-decoration: none; }
    a:hover { text-decoration: underline; }
</style>
