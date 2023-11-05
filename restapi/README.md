# Documentation for FitLayout REST API

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *http://localhost:8080/fitlayout-web*

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
*ArtifactApi* | [**refreshArtifact**](Apis/ArtifactApi.md#refreshartifact) | **GET** /api/r/{repoId}/artifact/refresh/{iri} | Recomputes the computed artifact properties
*AuthApi* | [**getUserInfo**](Apis/AuthApi.md#getuserinfo) | **GET** /api/auth/userInfo | Get current user information based on the credentials (Bearer JWT token) obtained
*QueryApi* | [**addQuery**](Apis/QueryApi.md#addquery) | **POST** /api/r/{repoId}/query | Adds a saved a query
*QueryApi* | [**deleteQuery**](Apis/QueryApi.md#deletequery) | **DELETE** /api/r/{repoId}/query/{id} | Deletes a saved query
*QueryApi* | [**getQuery**](Apis/QueryApi.md#getquery) | **GET** /api/r/{repoId}/query/{id} | Obtains a saved query
*QueryApi* | [**list**](Apis/QueryApi.md#list) | **GET** /api/r/{repoId}/query | Obtains all the saved queries
*RepositoryApi* | [**addNamespace**](Apis/RepositoryApi.md#addnamespace) | **PUT** /api/r/{repoId}/repository/namespaces/{prefix} | Adds a namespace definition for the given prefix
*RepositoryApi* | [**addQuadruple**](Apis/RepositoryApi.md#addquadruple) | **POST** /api/r/{repoId}/repository/add | Adds a new quadruple to the repository
*RepositoryApi* | [**addQuadruples**](Apis/RepositoryApi.md#addquadruples) | **POST** /api/r/{repoId}/repository/addQuads | Adds a list of new quadruple to the repository
*RepositoryApi* | [**addStatements**](Apis/RepositoryApi.md#addstatements) | **POST** /api/r/{repoId}/repository/statements | Imports (adds) statements to the repository
*RepositoryApi* | [**checkRepo**](Apis/RepositoryApi.md#checkrepo) | **GET** /api/r/{repoId}/repository/checkRepo | Checks the repository whether it exists and is properly initialized
*RepositoryApi* | [**clearNamespaces**](Apis/RepositoryApi.md#clearnamespaces) | **DELETE** /api/r/{repoId}/repository/namespaces | Removes all namespace declarations from the repository
*RepositoryApi* | [**deleteNamespace**](Apis/RepositoryApi.md#deletenamespace) | **DELETE** /api/r/{repoId}/repository/namespaces/{prefix} | Removes a namespace definition for the given prefix
*RepositoryApi* | [**deleteQuadruples**](Apis/RepositoryApi.md#deletequadruples) | **POST** /api/r/{repoId}/repository/deleteQuads | Removes a list of quadruples from the repository
*RepositoryApi* | [**deleteStatements**](Apis/RepositoryApi.md#deletestatements) | **DELETE** /api/r/{repoId}/repository/statements | Deletes statements from the repository
*RepositoryApi* | [**describeSubject**](Apis/RepositoryApi.md#describesubject) | **GET** /api/r/{repoId}/repository/describe/{iri} | Gets the RDF description for the given subject IRI
*RepositoryApi* | [**forceInitRepo**](Apis/RepositoryApi.md#forceinitrepo) | **GET** /api/r/{repoId}/repository/forceInitRepo | Re-initializes an empty repository with the necessary RDF metadata (schemas)
*RepositoryApi* | [**getContexts**](Apis/RepositoryApi.md#getcontexts) | **GET** /api/r/{repoId}/repository/contexts | Gets a list of contexts that have been defined for the repository
*RepositoryApi* | [**getNamespace**](Apis/RepositoryApi.md#getnamespace) | **GET** /api/r/{repoId}/repository/namespaces/{prefix} | Gets a namespace URI for the given prefix
*RepositoryApi* | [**getNamespaces**](Apis/RepositoryApi.md#getnamespaces) | **GET** /api/r/{repoId}/repository/namespaces | Gets a list of namespace declarations that have been defined for the repository
*RepositoryApi* | [**getStatements**](Apis/RepositoryApi.md#getstatements) | **GET** /api/r/{repoId}/repository/statements | Gets all RDF statements from the repository
*RepositoryApi* | [**getSubjectType**](Apis/RepositoryApi.md#getsubjecttype) | **GET** /api/r/{repoId}/repository/type/{iri} | Gets the assigned rdf:type IRI for the given subject IRI
*RepositoryApi* | [**getSubjectValue**](Apis/RepositoryApi.md#getsubjectvalue) | **GET** /api/r/{repoId}/repository/subject/{subjIri}/{propertyIri} | Gets the property value for the given subject and property IRIs
*RepositoryApi* | [**initRepo**](Apis/RepositoryApi.md#initrepo) | **GET** /api/r/{repoId}/repository/initRepo | Initializes an empty repository with the necessary RDF metadata (schemas)
*RepositoryApi* | [**query**](Apis/RepositoryApi.md#query) | **POST** /api/r/{repoId}/repository/query | Executes any SPARQL query on the underlying RDF repository
*RepositoryApi* | [**queryObject**](Apis/RepositoryApi.md#queryobject) | **GET** /api/r/{repoId}/repository/object/{iri} | Gets all triples for the given object IRI
*RepositoryApi* | [**querySubject**](Apis/RepositoryApi.md#querysubject) | **GET** /api/r/{repoId}/repository/subject/{iri} | Gets all triples for the given subject IRI
*RepositoryApi* | [**replaceStatements**](Apis/RepositoryApi.md#replacestatements) | **PUT** /api/r/{repoId}/repository/statements | Replaces all statements in the repository
*RepositoryApi* | [**selectQuery**](Apis/RepositoryApi.md#selectquery) | **POST** /api/r/{repoId}/repository/selectQuery | Executes a SPARQL SELECT query on the underlying RDF repository
*RepositoryApi* | [**touch**](Apis/RepositoryApi.md#touch) | **GET** /api/r/{repoId}/repository/touch | Updates the last access time of the given repository to current time
*RepositoryApi* | [**updateQuery**](Apis/RepositoryApi.md#updatequery) | **POST** /api/r/{repoId}/repository/updateQuery | Executes a SPARQL UPDATE query on the underlying RDF repository
*RepositoryOperatorApi* | [**repositoryListOperators**](Apis/RepositoryOperatorApi.md#repositorylistoperators) | **GET** /api/r/{repoId}/operator | Gets a list of available area tree operator services for the repository.
*RepositoryServiceApi* | [**getRepoServiceConfig**](Apis/RepositoryServiceApi.md#getreposerviceconfig) | **GET** /api/r/{repoId}/service/config | Gets the default configuration of an artifact service.
*RepositoryServiceApi* | [**repositoryGetServiceList**](Apis/RepositoryServiceApi.md#repositorygetservicelist) | **GET** /api/r/{repoId}/service | Gets a list of available artifact services for the repository.
*RepositoryServiceApi* | [**repositoryInvoke**](Apis/RepositoryServiceApi.md#repositoryinvoke) | **POST** /api/r/{repoId}/service | Invokes a service and returns the resulting artifact
*RunServiceApi* | [**renderJsonPage**](Apis/RunServiceApi.md#renderjsonpage) | **POST** /api/r/{repoId}/run/renderJson | Creates a new Page artifact from a JSON page description (e.g. obtained from a puppeteer backend or a client browser extension).
*ServiceApi* | [**getServiceConfig**](Apis/ServiceApi.md#getserviceconfig) | **GET** /api/service/config | Gets the default configuration of an artifact service.
*ServiceApi* | [**getServiceList**](Apis/ServiceApi.md#getservicelist) | **GET** /api/service | Gets a list of available artifact services.
*ServiceApi* | [**invoke**](Apis/ServiceApi.md#invoke) | **POST** /api/service | Invokes a service and returns the resulting artifact
*ServiceApi* | [**listOperators**](Apis/ServiceApi.md#listoperators) | **GET** /api/operator | Gets a list of available area tree operator services.
*ServiceApi* | [**ping**](Apis/ServiceApi.md#ping) | **GET** /api/service/ping | Returns 'ok'.
*TagsApi* | [**getTags**](Apis/TagsApi.md#gettags) | **GET** /api/r/{repoId}/tags | Reads a list of tags defined in the repository


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
 - [SavedQueryDTO](./Models/SavedQueryDTO.md)
 - [SelectQueryResult](./Models/SelectQueryResult.md)
 - [ServiceParams](./Models/ServiceParams.md)
 - [StorageStatus](./Models/StorageStatus.md)
 - [SubjectDescriptionResult](./Models/SubjectDescriptionResult.md)
 - [TagInfo](./Models/TagInfo.md)
 - [UserInfo](./Models/UserInfo.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="jwt"></a>
### jwt

- **Type**: HTTP bearer authentication (JWT)

