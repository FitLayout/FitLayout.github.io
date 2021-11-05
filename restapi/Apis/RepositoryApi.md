# RepositoryApi

All URIs are relative to *http://localhost:9080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addNamespace**](RepositoryApi.md#addNamespace) | **PUT** /api/r/{repoId}/repository/namespaces/{prefix} | Adds a namespace definition for the given prefix
[**addQuadruple**](RepositoryApi.md#addQuadruple) | **POST** /api/r/{repoId}/repository/add | Adds a new quadruple to the repository
[**checkRepo**](RepositoryApi.md#checkRepo) | **GET** /api/r/{repoId}/repository/checkRepo | Checks the repository whether it exists and is properly initialized
[**clearNamespaces**](RepositoryApi.md#clearNamespaces) | **DELETE** /api/r/{repoId}/repository/namespaces | Removes all namespace declarations from the repository
[**deleteNamespace**](RepositoryApi.md#deleteNamespace) | **DELETE** /api/r/{repoId}/repository/namespaces/{prefix} | Removes a namespace definition for the given prefix
[**describeSubject**](RepositoryApi.md#describeSubject) | **GET** /api/r/{repoId}/repository/describe/{iri} | Gets the RDF description for the given subject IRI
[**getNamespace**](RepositoryApi.md#getNamespace) | **GET** /api/r/{repoId}/repository/namespaces/{prefix} | Gets a namespace URI for the given prefix
[**getNamespaces**](RepositoryApi.md#getNamespaces) | **GET** /api/r/{repoId}/repository/namespaces | Gets a list of namespace declarations that have been defined for the repository
[**getSubjectType**](RepositoryApi.md#getSubjectType) | **GET** /api/r/{repoId}/repository/type/{iri} | Gets the assigned rdf:type IRI for the given subject IRI
[**getSubjectValue**](RepositoryApi.md#getSubjectValue) | **GET** /api/r/{repoId}/repository/subject/{subjIri}/{propertyIri} | Gets the property value for the given subject and property IRIs
[**initRepo**](RepositoryApi.md#initRepo) | **GET** /api/r/{repoId}/repository/initRepo | Initializes an empty repository with the necessary RDF metadata (schemas)
[**queryObject**](RepositoryApi.md#queryObject) | **GET** /api/r/{repoId}/repository/object/{iri} | Gets all triples for the given object IRI
[**querySubject**](RepositoryApi.md#querySubject) | **GET** /api/r/{repoId}/repository/subject/{iri} | Gets all triples for the given subject IRI
[**repositoryQuery**](RepositoryApi.md#repositoryQuery) | **POST** /api/r/{repoId}/repository/query | Executes a SPARQL SELECT query on the underlying RDF repository
[**touch**](RepositoryApi.md#touch) | **GET** /api/r/{repoId}/repository/touch | Updates the last access time of the given repository to current time


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

<a name="repositoryQuery"></a>
# **repositoryQuery**
> SelectQueryResult repositoryQuery(repoId, body)

Executes a SPARQL SELECT query on the underlying RDF repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
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

