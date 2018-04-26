# Eclipse Tips
Clone this repo and put your provider in the providers.json file. 

## providers.json
### "require-bundle": "org.eclipse.ui"
This bundle must be available in the IDE before your provider can be active. It is also the name of the subdirectory where your provider.json file must exist

### "version": "1.0.0"
The version of your provider. If you provide new tips then this version must be updated. The framework will only download new tips of the version has changed.

## provider.json
This file contains your provider definition and your tips.

{
  "provider": {
    "image": "data:image/png;base64,i..ggg==",
    "description": "Photon new and noteworthy",
    "id": "org.eclipse.jdt.tips",
    "expression": "<core expression>",
    "tips": [
      {
        "subject": "HTML Only Tip",
        "date": "2018-02-12",
        "html": "<valid html>"
      },
      {
        "subject": "HTML and Image",
        "date": "2018-01-21",
        "image": "data:image/png;base64,i...==",
        "ratio": 1.35,
        "maxHeight": 300,
        "actionId": "preferences",
        "html": "<h2>title</h2>The <b>DirectoryDialog</b> has.. etc.."
      },
      {
        "subject": "Eclipse Wiki Tip",
        "date": "2018-02-07",
        "maxWidth": 500,
        "url": "https://wiki.eclipse.org/Tip_of_the_Day/Eclipse_Tips/Json_Tip?action=render"
      }
    ]
  }
}
