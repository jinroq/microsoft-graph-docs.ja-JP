---
title: リスト privilegedRoleAssignments
description: 組織のすべてのロールの割り当てに対応する、privilegedRoleAssignment オブジェクトの一覧を取得します。
ms.openlocfilehash: 7642768348e2fff43f52c6865cabf85aa16ef893
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072491"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="8cee8-103">リスト privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="8cee8-103">List privilegedRoleAssignments</span></span>

> <span data-ttu-id="8cee8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cee8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cee8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cee8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cee8-106">組織のすべてのロールの割り当てに対応する、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8cee8-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="8cee8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8cee8-107">Permissions</span></span>
<span data-ttu-id="8cee8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cee8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8cee8-110">リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。</span><span class="sxs-lookup"><span data-stu-id="8cee8-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="8cee8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cee8-111">Permission type</span></span>      | <span data-ttu-id="8cee8-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cee8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cee8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cee8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8cee8-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cee8-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cee8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cee8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cee8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cee8-116">Not supported.</span></span>    |
|<span data-ttu-id="8cee8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cee8-117">Application</span></span> | <span data-ttu-id="8cee8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cee8-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cee8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cee8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8cee8-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8cee8-120">Optional query parameters</span></span>
<span data-ttu-id="8cee8-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8cee8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cee8-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cee8-122">Request headers</span></span>
| <span data-ttu-id="8cee8-123">名前</span><span class="sxs-lookup"><span data-stu-id="8cee8-123">Name</span></span>      |<span data-ttu-id="8cee8-124">説明</span><span class="sxs-lookup"><span data-stu-id="8cee8-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8cee8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cee8-125">Authorization</span></span>  | <span data-ttu-id="8cee8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8cee8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cee8-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cee8-128">Request body</span></span>
<span data-ttu-id="8cee8-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8cee8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cee8-130">応答</span><span class="sxs-lookup"><span data-stu-id="8cee8-130">Response</span></span>

<span data-ttu-id="8cee8-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8cee8-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="8cee8-132">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="8cee8-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8cee8-133">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cee8-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="8cee8-134">例</span><span class="sxs-lookup"><span data-stu-id="8cee8-134">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="8cee8-135">すべてのロールの割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="8cee8-135">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="8cee8-136">要求</span><span class="sxs-lookup"><span data-stu-id="8cee8-136">Request</span></span>
<span data-ttu-id="8cee8-137">次の使用例は、すべてのロールの割り当てを取得する要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="8cee8-137">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="8cee8-138">応答</span><span class="sxs-lookup"><span data-stu-id="8cee8-138">Response</span></span>
<span data-ttu-id="8cee8-139">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8cee8-139">The following example shows the response.</span></span> <span data-ttu-id="8cee8-140">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8cee8-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8cee8-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cee8-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```
### <a name="get-active-role-assignments"></a><span data-ttu-id="8cee8-142">アクティブなロールの割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="8cee8-142">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="8cee8-143">要求</span><span class="sxs-lookup"><span data-stu-id="8cee8-143">Request</span></span> 
<span data-ttu-id="8cee8-144">次の使用例は、クエリの有効なロールの割り当ての要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="8cee8-144">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="8cee8-145">応答</span><span class="sxs-lookup"><span data-stu-id="8cee8-145">Response</span></span>
<span data-ttu-id="8cee8-146">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8cee8-146">The following example shows the response.</span></span> <span data-ttu-id="8cee8-147">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8cee8-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8cee8-148">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cee8-148">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_62e90394-69f5-4237-9190-012177145e10",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "62e90394-69f5-4237-9190-012177145e10",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T17:38:49.563Z",
            "resultMessage": null
        }
  ]
}
```
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="8cee8-149">永続的な役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="8cee8-149">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="8cee8-150">要求</span><span class="sxs-lookup"><span data-stu-id="8cee8-150">Request</span></span> 
<span data-ttu-id="8cee8-151">次の例では、クエリの永続的な役割の割り当ての要求、``expirationDateTime``の値は、 ``null``。</span><span class="sxs-lookup"><span data-stu-id="8cee8-151">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="8cee8-152">応答</span><span class="sxs-lookup"><span data-stu-id="8cee8-152">Response</span></span>
<span data-ttu-id="8cee8-153">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8cee8-153">The following example shows the response.</span></span> <span data-ttu-id="8cee8-154">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8cee8-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8cee8-155">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cee8-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_44367163-eba1-44c3-98af-f5787879f96a",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="8cee8-156">対象となる役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="8cee8-156">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="8cee8-157">要求</span><span class="sxs-lookup"><span data-stu-id="8cee8-157">Request</span></span> 
<span data-ttu-id="8cee8-158">次の使用例は、アクティブおよび非アクティブなものも含めて、クエリ対象のロールの割り当ての要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="8cee8-158">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="8cee8-159">応答</span><span class="sxs-lookup"><span data-stu-id="8cee8-159">Response</span></span> 
<span data-ttu-id="8cee8-160">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8cee8-160">The following example shows the response.</span></span> <span data-ttu-id="8cee8-161">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8cee8-161">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8cee8-162">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cee8-162">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T18:42:26.823Z",
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_9360feb5-f418-4baa-8175-e2a00bac4301",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
