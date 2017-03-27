### programmercv Résumé Schema

The programmercv Résumé Standard is an open source [JSON Schema](http://json-schema.org/) Definition to store résumé data.

It is heavily influenced by the existing resume standards [FRESCA](https://github.com/fresh-standard/FRESCA) and [JSONResume](https://github.com/jsonresume/resume-schema), then cherry-picked and adopted to the needs and requirements of [programmercv](https://prtfl.io) and [RésuméExporter](https://github.com/prtflio/resume_exporter).

## Why?

![standards](http://imgs.xkcd.com/comics/standards.png)

Not really intended to set *the standard* for résumés, nor to replace existing ones. In fact, programmercv and RésuméExporter are designed to work with FRESCA- and JSONResume-based schemas. But both schema definitions were missing some elements, and we needed a clearly defined schema definition for [programmercv](https://prtfl.io) and the programmercv jekyll theme (coming soon), in a public place, where people can read, understand, discuss, change and use it.

- [**programmercv Resume Schema Definition**](schema.json)
- [**Example Resume**](example.json)
- [**Validate your json data**](https://jsonschemalint.com/#/version/draft-04/markup/json?gist=76f130ed99a573f5eaf2aca60eeaefcc)

Structure Overview:

```javascript
{
  "meta": {
    "format": "",
    "version": ""
  },

  "basics": {
    "name": "",
    "label": "",
    "image": "",
    "summary": "",
    "contact": {
      "email": "",
      "phone": "",
      "website": "",
      "location": "",
      "social": [{
        "network": "",
        "user": "",
        "url": ""
      }]
    }
  },

  "employment": {
    "summary": "",
    "history": [{          
      "employer": "",
      "position": "",
      "url": "",
      "startDate": "",
      "endDate": "",
      "summary": "",
      "location": "",
      "highlights": [""],
      "keywords": [""]
    }]
  },

  "education": {
    "summary": "",
    "history":[{
      "institution": "",
      "fieldOfStudy": "",
      "degree": "",
      "startDate": "",
      "endDate": "",
      "grade": "",
      "url": "",
      "summary": "",
      "location": "",
      "curriculum": [""],
      "highlights": [""],
      "keywords": [""]
    }]
  },

  "projects": {
    "summary": "",
    "history": [{
      "title": "",
      "description": "",
      "url": "",
      "repo": "",
      "startDate": "",
      "endDate": "",
      "category": "",
      "images": [{            
        "thumbnail": "",
        "big": ""
      }],
      "roles": [""],
      "highlights": [""],
      "keywords": [""]
    }]
  },

  "openSource": {
    "summary": "",
    "history": [{
      "title": "",
      "description": "",
      "url": "",
      "repo": "",
      "startDate": "",
      "endDate": "",
      "category": "",
      "roles": [""],
      "highlights": [""],
      "keywords": [""]
    }]
  },

  "skills": {
    "summary": "",
    "sets": [{
      "name": "",
      "description": "",
      "keywords": [""]
    }]
  },

  "qualifications": {
    "summary": "",
    "history": [{
      "category": "",
      "title": "",
      "startDate": "",
      "endDate": "",
      "from": "",
      "summary": "",
      "url": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "recognition": {
    "summary": "",
    "history": [{
      "category": "",
      "title": "",
      "startDate": "",
      "endDate": "",
      "from": "",
      "summary": "",
      "url": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "writing": {
    "summary": "",
    "history": [{
      "title": "",
      "category": "",
      "date": "",
      "url": "",
      "publisher": "",
      "summary": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "reading": {
    "summary": "",
    "history": [{
      "title": "",
      "category": "",
      "url": "",
      "author": "",
      "date": "",
      "summary": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "speaking": {
    "summary": "",
    "history": [{
      "title": "",
      "event": "",
      "location": "",
      "url": "",
      "date": "",
      "summary": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "patents": {
    "summary": "",
    "history": [{
      "title": "",
      "url": "",
      "number": "",
      "status": "",
      "description": "",
      "date": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "languages": {
    "summary": "",
    "history": [{
      "language": "",
      "level": "",
      "years": ""
    }]
  },

  "interests": {
    "summary": "",
    "history": [{
      "name": "",
      "description": ""
    }]
  },

  "extracurriculars": {
    "summary": "",
    "history": [{
      "title": "",
      "summary": "",
      "category": "",
      "url": "",
      "location": "",
      "startDate": "",
      "endDate": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "affiliations": {
    "summary": "",
    "history": [{
      "category": "",
      "organization": "",
      "roles": [],
      "url": "",
      "startDate": "",
      "endDate": "",
      "summary": "",
      "location": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "governance": {
    "summary": "",
    "history": [{
      "summary": "",
      "category": "",
      "url": "",
      "roles": [],
      "organization": "",
      "startDate": "",
      "endDate": "",
      "keywords": [],
      "highlights": []
    }]
  },

  "service": {
    "summary": "",
    "history": [{
      "category": "",
      "organization": "",
      "roles": [],
      "url": "",
      "startDate": "",
      "endDate": "",
      "summary": "",
      "location": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "references": {
    "summary": "",
    "history": [{
      "name": "",
      "role": "",
      "company": "",
      "summary": ""
    }]
  },

  "disposition": {
    "summary": "",
    "history": [{
      "travel": 20,
      "authorization": "",
      "commitment": [],
      "remote": true,
      "relocation": {
        "willing": true,
        "destinations": []
      }
    }]
  }
}

```