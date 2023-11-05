# RepositoryServiceApi

All URIs are relative to *http://localhost:8080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getRepoServiceConfig**](RepositoryServiceApi.md#getRepoServiceConfig) | **GET** /api/r/{repoId}/service/config | Gets the default configuration of an artifact service.
[**repositoryGetServiceList**](RepositoryServiceApi.md#repositoryGetServiceList) | **GET** /api/r/{repoId}/service | Gets a list of available artifact services for the repository.
[**repositoryInvoke**](RepositoryServiceApi.md#repositoryInvoke) | **POST** /api/r/{repoId}/service | Invokes a service and returns the resulting artifact


<a name="getRepoServiceConfig"></a>
# **getRepoServiceConfig**
> ServiceParams getRepoServiceConfig(repoId, id)

Gets the default configuration of an artifact service.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **id** | **String**|  | [optional] [default to null]

### Return type

[**ServiceParams**](../Models/ServiceParams.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="repositoryGetServiceList"></a>
# **repositoryGetServiceList**
> List repositoryGetServiceList(repoId)

Gets a list of available artifact services for the repository.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**List**](../Models/ArtifactServiceDescr.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="repositoryInvoke"></a>
# **repositoryInvoke**
> repositoryInvoke(repoId, ServiceParams)

Invokes a service and returns the resulting artifact

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **ServiceParams** | [**ServiceParams**](../Models/ServiceParams.md)|  | [optional]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/ld+json, text/turtle, application/rdf+xml, application/n-triples, application/n-quads

