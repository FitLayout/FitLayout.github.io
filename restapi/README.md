# Documentation for FitLayout REST API

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints


Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AdminApi* | [**createRepository**](Apis/AdminApi.md#createrepository) | **POST** /api/repository | Creates a new repository.
*AdminApi* | [**deleteRepository**](Apis/AdminApi.md#deleterepository) | **DELETE** /api/repository/{repoId} | Deletes a repository identified by its ID.
*AdminApi* | [**getRepositoryInfo**](Apis/AdminApi.md#getrepositoryinfo) | **GET** /api/repository/{repoId} | Gets information about a repository identified by its ID.
*AdminApi* | [**listAllRepositories**](Apis/AdminApi.md#listallrepositories) | **GET** /api/repository/all | Gets a list of all available repositories (admin only).
*AdminApi* | [**listRepositories**](Apis/AdminApi.md#listrepositories) | **GET** /api/repository | Gets a list of available repositories for current user.
*AdminApi* | [**sendRepositoriesReminder**](Apis/AdminApi.md#sendrepositoriesreminder) | **GET** /api/repository/remind/{email} | Sends an e-mail reminder containing all repositories that have the given e-mail assigned
*AdminApi* | [**status**](Apis/AdminApi.md#status) | **GET** /api/repository/status | Gets overall storage status.
*AdminApi* | [**updateRepositoryInfo**](Apis/AdminApi.md#updaterepositoryinfo) | **PUT** /api/repository/{repoId} | Gets information about a repository identified by its ID.
*ArtifactApi* | [**clear**](Apis/ArtifactApi.md#clear) | **DELETE** /api/r/{repoId}/artifact/clear | Clears the repository - deletes all artifacts and metadata
*ArtifactApi* | [**createArtifact**](Apis/ArtifactApi.md#createartifact) | **POST** /api/r/{repoId}/artifact/create | Creates a new artifact by invoking a service.
*ArtifactApi* | [**deleteArtifact**](Apis/ArtifactApi.md#deleteartifact) | **DELETE** /api/r/{repoId}/artifact/item/{iri} | Deletes an artifact identified by its IRI
*ArtifactApi* | [**getArtifact**](Apis/ArtifactApi.md#getartifact) | **GET** /api/r/{repoId}/artifact/item/{iri} | Gets a complete artifact including its contents identified by its IRI
*ArtifactApi* | [**getArtifactInfo**](Apis/ArtifactApi.md#getartifactinfo) | **GET** /api/r/{repoId}/artifact/info/{iri} | Retrieves information about an artifact identified by its IRI (artifact content not included).
*ArtifactApi* | [**getArtifactsInfo**](Apis/ArtifactApi.md#getartifactsinfo) | **GET** /api/r/{repoId}/artifact | Retrieves information about all artifacts in the repository (artifact contents not included).
*ArtifactApi* | [**listArtifacts**](Apis/ArtifactApi.md#listartifacts) | **GET** /api/r/{repoId}/artifact/list | Gets a list of artifact IRIs.
*AuthApi* | [**getUserInfo**](Apis/AuthApi.md#getuserinfo) | **GET** /api/auth/userInfo | Get current user information based on the credentials (Bearer JWT token) obtained
*RepositoryApi* | [**addQuadruple**](Apis/RepositoryApi.md#addquadruple) | **POST** /api/r/{repoId}/repository/add | Adds a new quadruple to the repository
*RepositoryApi* | [**checkRepo**](Apis/RepositoryApi.md#checkrepo) | **GET** /api/r/{repoId}/repository/checkRepo | Checks the repository whether it exists and is properly initialized
*RepositoryApi* | [**describeSubject**](Apis/RepositoryApi.md#describesubject) | **GET** /api/r/{repoId}/repository/describe/{iri} | Gets the RDF description for the given subject IRI
*RepositoryApi* | [**getSubjectType**](Apis/RepositoryApi.md#getsubjecttype) | **GET** /api/r/{repoId}/repository/type/{iri} | Gets the assigned rdf:type IRI for the given subject IRI
*RepositoryApi* | [**getSubjectValue**](Apis/RepositoryApi.md#getsubjectvalue) | **GET** /api/r/{repoId}/repository/subject/{subjIri}/{propertyIri} | Gets the property value for the given subject and property IRIs
*RepositoryApi* | [**initRepo**](Apis/RepositoryApi.md#initrepo) | **GET** /api/r/{repoId}/repository/initRepo | Initializes an empty repository with the necessary RDF metadata (schemas)
*RepositoryApi* | [**queryObject**](Apis/RepositoryApi.md#queryobject) | **GET** /api/r/{repoId}/repository/object/{iri} | Gets all triples for the given object IRI
*RepositoryApi* | [**querySubject**](Apis/RepositoryApi.md#querysubject) | **GET** /api/r/{repoId}/repository/subject/{iri} | Gets all triples for the given subject IRI
*RepositoryApi* | [**repositoryQuery**](Apis/RepositoryApi.md#repositoryquery) | **POST** /api/r/{repoId}/repository/query | Executes a SPARQL SELECT query on the underlying RDF repository
*RepositoryApi* | [**touch**](Apis/RepositoryApi.md#touch) | **GET** /api/r/{repoId}/repository/touch | Updates the last access time of the given repository to current time
*ServiceApi* | [**getServiceConfig**](Apis/ServiceApi.md#getserviceconfig) | **GET** /api/service/config | Gets the default configuration of an artifact service.
*ServiceApi* | [**getServiceList**](Apis/ServiceApi.md#getservicelist) | **GET** /api/service | Gets a list of available artifact services.
*ServiceApi* | [**invoke**](Apis/ServiceApi.md#invoke) | **POST** /api/service | Invokes a service and returns the resulting artifact
*ServiceApi* | [**listOperators**](Apis/ServiceApi.md#listoperators) | **GET** /api/operator | Gets a list of available area tree operator services.
*ServiceApi* | [**ping**](Apis/ServiceApi.md#ping) | **GET** /api/service/ping | Returns 'ok'.


<a name="documentation-for-models"></a>
## Documentation for Models

 - [ArtifactServiceDescr](./Models/ArtifactServiceDescr.md)
 - [ParamBooleanDescr](./Models/ParamBooleanDescr.md)
 - [ParamDescr](./Models/ParamDescr.md)
 - [ParamFloatDescr](./Models/ParamFloatDescr.md)
 - [ParamIntDescr](./Models/ParamIntDescr.md)
 - [ParamStringDescr](./Models/ParamStringDescr.md)
 - [ParametrizedServiceDescr](./Models/ParametrizedServiceDescr.md)
 - [QuadrupleData](./Models/QuadrupleData.md)
 - [RepositoryInfo](./Models/RepositoryInfo.md)
 - [ResultBinding](./Models/ResultBinding.md)
 - [ResultBody](./Models/ResultBody.md)
 - [ResultErrorMessage](./Models/ResultErrorMessage.md)
 - [ResultHeader](./Models/ResultHeader.md)
 - [ResultValue](./Models/ResultValue.md)
 - [SelectQueryResult](./Models/SelectQueryResult.md)
 - [ServiceParams](./Models/ServiceParams.md)
 - [StorageStatus](./Models/StorageStatus.md)
 - [SubjectDescriptionResult](./Models/SubjectDescriptionResult.md)
 - [UserInfo](./Models/UserInfo.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="jwt"></a>
### jwt

- **Type**: HTTP basic authentication

