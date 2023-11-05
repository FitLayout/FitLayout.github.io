# RepositoryOperatorApi

All URIs are relative to *http://localhost:8080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**repositoryListOperators**](RepositoryOperatorApi.md#repositoryListOperators) | **GET** /api/r/{repoId}/operator | Gets a list of available area tree operator services for the repository.


<a name="repositoryListOperators"></a>
# **repositoryListOperators**
> List repositoryListOperators(repoId)

Gets a list of available area tree operator services for the repository.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**List**](../Models/ParametrizedServiceDescr.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

