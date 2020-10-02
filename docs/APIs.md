# APIs for bibliometric information

This is a list of APIs that provide bibliometric information. 

| API       | Microsoft    | CrossRef     | Elsevier     | ArXiv        | Europe PMC   | IEEExplore   | Semantic Scholar API | Mendeley | Springer |
|-----------|--------------|--------------|--------------|--------------|--------------|--------------|----------------------|----------|----------|
| Website   | [URL](https://www.microsoft.com/en-us/research/project/academic-knowledge/)  | [URL](https://search.crossref.org/) | [URL](https://dev.elsevier.com/) | [URL](https://arxiv.org/help/api/index) | [URL](http://europepmc.org/RestfulWebService) | [URL](https://developer.ieee.org/getting_started) | [URL](https://api.semanticscholar.org/) | [URL](https://dev.mendeley.com/) |  [URL](https://dev.springernature.com/) |
| Register  | [URL](https://www.microsoft.com/en-us/research/project/academic-knowledge/) | [URL](https://github.com/CrossRef/rest-api-doc#good-manners--more-reliable-service) | [URL](https://dev.elsevier.com/apikey/manage) | [URL](https://arxiv.org/help/api/tou) | [URL](http://europepmc.org/RestfulWebService) | [URL](https://developer.ieee.org/member/register) | [URL](http://s2-public-api-prod.us-west-2.elasticbeanstalk.com/license/) | [URL](https://dev.mendeley.com/reference/topics/authorization_overview.html) | [URL]() |
| Documentation | [URL](https://docs.microsoft.com/en-us/academic-services/project-academic-knowledge/introduction) | [URL](https://github.com/CrossRef/rest-api-doc) | [URL](https://dev.elsevier.com/api_docs.html) | [URL](https://arxiv.org/help/api/user-manual) | [URL](http://europepmc.org/RestfulWebService#!/Europe32PMC32Articles32RESTful32API) | [URL](https://developer.ieee.org/docs) | [URL](https://api.semanticscholar.org/) | [URL](https://github.com/Mendeley/mendeley-python-sdk) | [URL](https://dev.springernature.com/restfuloperations) |
|  Free | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
|  DOI   | ❌ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
|  #Citations   | ✅ | ✅ | ✅ | ❌ | ✅ | ✅ | ✅ | ❌ | ❌ |
|  Citation IDs   | ❌ | ✅ | ✅ | ❌ | ❌ | ❌ | ✅ | ❌ | ❌ |
|  #References   | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ | ✅ | ❌ | ❌ |
|  Reference IDs   | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ | ✅ | ❌ | ❌ |
|  Journal Indicators | ❓ | ✅ | ✅ | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ |
|  Data Format   | JSON | JSON | JSON | XML | XML, JSON, or DC | XML, or JSON | HTML | JSON | XML, or JSON |
|  Limitations   | Not many papers |  |  | Only ArXiv papers | Not much info | Not much info |  | Not much info | Not much info |

# Examples 

## Microsoft academic

Get paper information: 

```html
https://api.labs.cognitive.microsoft.com/academic/v1.0/evaluate?expr=And(Composite(AA.AuN=='{}'),Y=[{},{}],Ti='{}',Ty='{}')&model=latest&count=10&offset=0&attributes=Id,Ty,Ti,Y,CC,CitCon,ECC,AA.AfId,AA.AfN,AA.AuId,AA.AuN,AA.DAuN,AA.DAfN,AA.S,AW,BT,C.CId,C.CN,D,DN,DOI,F.DFN,F.FId,F.FN,FamId,FP,I,J.JId,J.JN,LP,PB,Pt,RId,S,Ti,V,VFN,VSN,W,Y
```