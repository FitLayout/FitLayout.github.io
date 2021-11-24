# ArtifactApi

All URIs are relative to *http://localhost:9080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**clear**](ArtifactApi.md#clear) | **DELETE** /api/r/{repoId}/artifact/clear | Clears the repository - deletes all artifacts and metadata
[**createArtifact**](ArtifactApi.md#createArtifact) | **POST** /api/r/{repoId}/artifact/create | Creates a new artifact by invoking a service.
[**deleteArtifact**](ArtifactApi.md#deleteArtifact) | **DELETE** /api/r/{repoId}/artifact/item/{iri} | Deletes an artifact identified by its IRI
[**getArtifact**](ArtifactApi.md#getArtifact) | **GET** /api/r/{repoId}/artifact/item/{iri} | Gets a complete artifact including its contents identified by its IRI
[**getArtifactInfo**](ArtifactApi.md#getArtifactInfo) | **GET** /api/r/{repoId}/artifact/info/{iri} | Retrieves information about an artifact identified by its IRI (artifact content not included).
[**getArtifactsInfo**](ArtifactApi.md#getArtifactsInfo) | **GET** /api/r/{repoId}/artifact | Retrieves information about all artifacts in the repository (artifact contents not included).
[**listArtifacts**](ArtifactApi.md#listArtifacts) | **GET** /api/r/{repoId}/artifact/list | Gets a list of artifact IRIs.
[**refreshArtifact**](ArtifactApi.md#refreshArtifact) | **GET** /api/r/{repoId}/artifact/refresh/{iri} | Recomputes the computed artifact properties


<a name="clear"></a>
# **clear**
> ResultValue clear(repoId)

Clears the repository - deletes all artifacts and metadata

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

<a name="createArtifact"></a>
# **createArtifact**
> ResultValue createArtifact(repoId, ServiceParams)

Creates a new artifact by invoking a service.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **ServiceParams** | [**ServiceParams**](../Models/ServiceParams.md)|  | [optional]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="deleteArtifact"></a>
# **deleteArtifact**
> ResultValue deleteArtifact(repoId, iri)

Deletes an artifact identified by its IRI

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

<a name="getArtifact"></a>
# **getArtifact**
> getArtifact(repoId, iri)

Gets a complete artifact including its contents identified by its IRI

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **iri** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/ld+json, text/turtle, application/rdf+xml, text/xml, text/html, image/png, application/json

<a name="getArtifactInfo"></a>
# **getArtifactInfo**
> getArtifactInfo(repoId, iri)

Retrieves information about an artifact identified by its IRI (artifact content not included).

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **iri** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/ld+json, text/turtle, application/rdf+xml, application/json

<a name="getArtifactsInfo"></a>
# **getArtifactsInfo**
> getArtifactsInfo(repoId)

Retrieves information about all artifacts in the repository (artifact contents not included).

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/ld+json, text/turtle, application/rdf+xml, application/json

<a name="listArtifacts"></a>
# **listArtifacts**
> List listArtifacts(repoId)

Gets a list of artifact IRIs.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**List**](../Models/string.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="refreshArtifact"></a>
# **refreshArtifact**
> ResultValue refreshArtifact(repoId, iri)

Recomputes the computed artifact properties

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

