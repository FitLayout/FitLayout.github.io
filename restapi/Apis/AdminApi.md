# AdminApi

All URIs are relative to *http://localhost:8080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createRepository**](AdminApi.md#createRepository) | **POST** /api/repository | Creates a new repository.
[**deleteRepository**](AdminApi.md#deleteRepository) | **DELETE** /api/repository/{repoId} | Deletes a repository identified by its ID.
[**getRepositoryInfo**](AdminApi.md#getRepositoryInfo) | **GET** /api/repository/{repoId} | Gets information about a repository identified by its ID.
[**listAllRepositories**](AdminApi.md#listAllRepositories) | **GET** /api/repository/all | Gets a list of all available repositories (admin only).
[**listRepositories**](AdminApi.md#listRepositories) | **GET** /api/repository | Gets a list of available repositories for current user.
[**sendRepositoriesReminder**](AdminApi.md#sendRepositoriesReminder) | **GET** /api/repository/remind/{email} | Sends an e-mail reminder containing all repositories that have the given e-mail assigned
[**status**](AdminApi.md#status) | **GET** /api/repository/status | Gets overall storage status.
[**updateRepositoryInfo**](AdminApi.md#updateRepositoryInfo) | **PUT** /api/repository/{repoId} | Gets information about a repository identified by its ID.


<a name="createRepository"></a>
# **createRepository**
> RepositoryInfo createRepository(RepositoryInfo)

Creates a new repository.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **RepositoryInfo** | [**RepositoryInfo**](../Models/RepositoryInfo.md)|  | [optional]

### Return type

[**RepositoryInfo**](../Models/RepositoryInfo.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="deleteRepository"></a>
# **deleteRepository**
> ResultValue deleteRepository(repoId)

Deletes a repository identified by its ID.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**|  | [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getRepositoryInfo"></a>
# **getRepositoryInfo**
> RepositoryInfo getRepositoryInfo(repoId)

Gets information about a repository identified by its ID.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**|  | [default to null]

### Return type

[**RepositoryInfo**](../Models/RepositoryInfo.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listAllRepositories"></a>
# **listAllRepositories**
> List listAllRepositories()

Gets a list of all available repositories (admin only).

### Parameters
This endpoint does not need any parameter.

### Return type

[**List**](../Models/RepositoryInfo.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listRepositories"></a>
# **listRepositories**
> List listRepositories()

Gets a list of available repositories for current user.

### Parameters
This endpoint does not need any parameter.

### Return type

[**List**](../Models/RepositoryInfo.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="sendRepositoriesReminder"></a>
# **sendRepositoriesReminder**
> ResultValue sendRepositoriesReminder(email)

Sends an e-mail reminder containing all repositories that have the given e-mail assigned

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **String**|  | [default to null]

### Return type

[**ResultValue**](../Models/ResultValue.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="status"></a>
# **status**
> StorageStatus status()

Gets overall storage status.

### Parameters
This endpoint does not need any parameter.

### Return type

[**StorageStatus**](../Models/StorageStatus.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="updateRepositoryInfo"></a>
# **updateRepositoryInfo**
> RepositoryInfo updateRepositoryInfo(repoId, RepositoryInfo)

Gets information about a repository identified by its ID.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**|  | [default to null]
 **RepositoryInfo** | [**RepositoryInfo**](../Models/RepositoryInfo.md)|  | [optional]

### Return type

[**RepositoryInfo**](../Models/RepositoryInfo.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

