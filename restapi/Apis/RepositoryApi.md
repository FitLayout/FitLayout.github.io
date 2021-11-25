# RepositoryApi

All URIs are relative to *http://localhost:9080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addNamespace**](RepositoryApi.md#addNamespace) | **PUT** /api/r/{repoId}/repository/namespaces/{prefix} | Adds a namespace definition for the given prefix
[**addQuadruple**](RepositoryApi.md#addQuadruple) | **POST** /api/r/{repoId}/repository/add | Adds a new quadruple to the repository
[**addQuadruples**](RepositoryApi.md#addQuadruples) | **POST** /api/r/{repoId}/repository/addQuads | Adds a list of new quadruple to the repository
[**addStatements**](RepositoryApi.md#addStatements) | **POST** /api/r/{repoId}/repository/statements | Imports statements to the repository
[**checkRepo**](RepositoryApi.md#checkRepo) | **GET** /api/r/{repoId}/repository/checkRepo | Checks the repository whether it exists and is properly initialized
[**clearNamespaces**](RepositoryApi.md#clearNamespaces) | **DELETE** /api/r/{repoId}/repository/namespaces | Removes all namespace declarations from the repository
[**deleteNamespace**](RepositoryApi.md#deleteNamespace) | **DELETE** /api/r/{repoId}/repository/namespaces/{prefix} | Removes a namespace definition for the given prefix
[**deleteQuadruples**](RepositoryApi.md#deleteQuadruples) | **POST** /api/r/{repoId}/repository/deleteQuads | Removes a list of quadruples from the repository
[**deleteStatements**](RepositoryApi.md#deleteStatements) | **DELETE** /api/r/{repoId}/repository/statements | Deletes statements from the repository
[**describeSubject**](RepositoryApi.md#describeSubject) | **GET** /api/r/{repoId}/repository/describe/{iri} | Gets the RDF description for the given subject IRI
[**getContexts**](RepositoryApi.md#getContexts) | **GET** /api/r/{repoId}/repository/contexts | Gets a list of contexts that have been defined for the repository
[**getNamespace**](RepositoryApi.md#getNamespace) | **GET** /api/r/{repoId}/repository/namespaces/{prefix} | Gets a namespace URI for the given prefix
[**getNamespaces**](RepositoryApi.md#getNamespaces) | **GET** /api/r/{repoId}/repository/namespaces | Gets a list of namespace declarations that have been defined for the repository
[**getStatements**](RepositoryApi.md#getStatements) | **GET** /api/r/{repoId}/repository/statements | Gets all RDF statements from the repository
[**getSubjectType**](RepositoryApi.md#getSubjectType) | **GET** /api/r/{repoId}/repository/type/{iri} | Gets the assigned rdf:type IRI for the given subject IRI
[**getSubjectValue**](RepositoryApi.md#getSubjectValue) | **GET** /api/r/{repoId}/repository/subject/{subjIri}/{propertyIri} | Gets the property value for the given subject and property IRIs
[**initRepo**](RepositoryApi.md#initRepo) | **GET** /api/r/{repoId}/repository/initRepo | Initializes an empty repository with the necessary RDF metadata (schemas)
[**query**](RepositoryApi.md#query) | **POST** /api/r/{repoId}/repository/query | Executes any SPARQL query on the underlying RDF repository
[**queryObject**](RepositoryApi.md#queryObject) | **GET** /api/r/{repoId}/repository/object/{iri} | Gets all triples for the given object IRI
[**querySubject**](RepositoryApi.md#querySubject) | **GET** /api/r/{repoId}/repository/subject/{iri} | Gets all triples for the given subject IRI
[**selectQuery**](RepositoryApi.md#selectQuery) | **POST** /api/r/{repoId}/repository/selectQuery | Executes a SPARQL SELECT query on the underlying RDF repository
[**touch**](RepositoryApi.md#touch) | **GET** /api/r/{repoId}/repository/touch | Updates the last access time of the given repository to current time
[**updateQuery**](RepositoryApi.md#updateQuery) | **POST** /api/r/{repoId}/repository/updateQuery | Executes a SPARQL UPDATE query on the underlying RDF repository


<a name="addNamespace"></a>
# **addNamespace**
> ResultValue addNamespace(repoId, prefix, body)

Adds a namespace definition for the given prefix

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **prefix** | **String**|  | [default to null]
 **body** | **String**|  | [optional]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: text/plain
- **Accept**: application/json

<a name="addQuadruple"></a>
# **addQuadruple**
> ResultValue addQuadruple(repoId, QuadrupleData)

Adds a new quadruple to the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **QuadrupleData** | [**QuadrupleData**](../Models/QuadrupleData.md)|  | [optional]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="addQuadruples"></a>
# **addQuadruples**
> ResultValue addQuadruples(repoId, QuadrupleData)

Adds a list of new quadruple to the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **QuadrupleData** | [**List**](../Models/QuadrupleData.md)|  | [optional]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="addStatements"></a>
# **addStatements**
> ResultValue addStatements(repoId, baseURI, context, body)

Imports statements to the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **baseURI** | **String**|  | [optional] [default to null]
 **context** | **String**|  | [optional] [default to null]
 **body** | **Object**|  | [optional]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/ld+json, text/turtle, application/rdf+xml, application/n-triples, application/n-quads
- **Accept**: application/json

<a name="checkRepo"></a>
# **checkRepo**
> ResultValue checkRepo(repoId)

Checks the repository whether it exists and is properly initialized

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="clearNamespaces"></a>
# **clearNamespaces**
> ResultValue clearNamespaces(repoId)

Removes all namespace declarations from the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="deleteNamespace"></a>
# **deleteNamespace**
> ResultValue deleteNamespace(repoId, prefix)

Removes a namespace definition for the given prefix

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **prefix** | **String**|  | [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="deleteQuadruples"></a>
# **deleteQuadruples**
> ResultValue deleteQuadruples(repoId, QuadrupleData)

Removes a list of quadruples from the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **QuadrupleData** | [**List**](../Models/QuadrupleData.md)|  | [optional]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="deleteStatements"></a>
# **deleteStatements**
> ResultValue deleteStatements(repoId, context, obj, pred, subj)

Deletes statements from the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **context** | **String**|  | [optional] [default to null]
 **obj** | **String**|  | [optional] [default to null]
 **pred** | **String**|  | [optional] [default to null]
 **subj** | **String**|  | [optional] [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="describeSubject"></a>
# **describeSubject**
> SubjectDescriptionResult describeSubject(repoId, iri)

Gets the RDF description for the given subject IRI

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **iri** | **String**|  | [default to null]

### Return type

[**SubjectDescriptionResult**](../Models/SubjectDescriptionResult.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getContexts"></a>
# **getContexts**
> SelectQueryResult getContexts(repoId)

Gets a list of contexts that have been defined for the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**SelectQueryResult**](../Models/SelectQueryResult.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getNamespace"></a>
# **getNamespace**
> getNamespace(repoId, prefix)

Gets a namespace URI for the given prefix

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **prefix** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain

<a name="getNamespaces"></a>
# **getNamespaces**
> SelectQueryResult getNamespaces(repoId)

Gets a list of namespace declarations that have been defined for the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**SelectQueryResult**](../Models/SelectQueryResult.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getStatements"></a>
# **getStatements**
> getStatements(repoId, context, obj, pred, subj)

Gets all RDF statements from the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **context** | **String**|  | [optional] [default to null]
 **obj** | **String**|  | [optional] [default to null]
 **pred** | **String**|  | [optional] [default to null]
 **subj** | **String**|  | [optional] [default to null]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/ld+json, text/turtle, application/rdf+xml, application/n-triples, application/n-quads, application/json

<a name="getSubjectType"></a>
# **getSubjectType**
> ResultValue getSubjectType(repoId, iri)

Gets the assigned rdf:type IRI for the given subject IRI

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **iri** | **String**|  | [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getSubjectValue"></a>
# **getSubjectValue**
> ResultBinding getSubjectValue(repoId, propertyIri, subjIri)

Gets the property value for the given subject and property IRIs

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **propertyIri** | **String**|  | [default to null]
 **subjIri** | **String**|  | [default to null]

### Return type

[**ResultBinding**](../Models/ResultBinding.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="initRepo"></a>
# **initRepo**
> ResultValue initRepo(repoId)

Initializes an empty repository with the necessary RDF metadata (schemas)

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="query"></a>
# **query**
> SelectQueryResult query(repoId, limit, offset, body)

Executes any SPARQL query on the underlying RDF repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **limit** | **Long**|  | [optional] [default to 100]
 **offset** | **Long**|  | [optional] [default to 0]
 **body** | **String**|  | [optional]

### Return type

[**SelectQueryResult**](../Models/SelectQueryResult.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/sparql-query
- **Accept**: application/json, application/ld+json, text/turtle, application/rdf+xml, application/n-triples, application/n-quads, text/boolean, text/xml

<a name="queryObject"></a>
# **queryObject**
> SelectQueryResult queryObject(repoId, iri, limit)

Gets all triples for the given object IRI

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **iri** | **String**|  | [default to null]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**SelectQueryResult**](../Models/SelectQueryResult.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="querySubject"></a>
# **querySubject**
> SelectQueryResult querySubject(repoId, iri, limit)

Gets all triples for the given subject IRI

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **iri** | **String**|  | [default to null]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**SelectQueryResult**](../Models/SelectQueryResult.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="selectQuery"></a>
# **selectQuery**
> SelectQueryResult selectQuery(repoId, limit, offset, body)

Executes a SPARQL SELECT query on the underlying RDF repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **limit** | **Long**|  | [optional] [default to 100]
 **offset** | **Long**|  | [optional] [default to 0]
 **body** | **String**|  | [optional]

### Return type

[**SelectQueryResult**](../Models/SelectQueryResult.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/sparql-query
- **Accept**: application/json

<a name="touch"></a>
# **touch**
> ResultValue touch(repoId)

Updates the last access time of the given repository to current time

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="updateQuery"></a>
# **updateQuery**
> ResultValue updateQuery(repoId, body)

Executes a SPARQL UPDATE query on the underlying RDF repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **body** | **String**|  | [optional]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/sparql-query
- **Accept**: application/json

