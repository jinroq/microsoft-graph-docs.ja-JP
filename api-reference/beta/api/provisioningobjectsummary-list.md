---
title: リストのプロビジョニングオブジェクトの概要
description: テナントで発生したすべてのプロビジョニングイベントを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 55e61b786fb144f23673d78cd756281daa15990a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412412"
---
# <a name="list-provisioningobjectsummary"></a><span data-ttu-id="6d988-103">リストのプロビジョニングオブジェクトの概要</span><span class="sxs-lookup"><span data-stu-id="6d988-103">List provisioningObjectSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d988-104">テナントで発生したすべてのプロビジョニングイベントを取得します。たとえば、ターゲットアプリケーションのグループの削除や、ユーザーアカウントを人事システムからプロビジョニングするときのユーザーの作成などです。</span><span class="sxs-lookup"><span data-stu-id="6d988-104">Get all provisioning events that occurred in your tenant, such as the deletion of a group in a target application or the creation of a user when provisioning user accounts from your HR system.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6d988-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d988-105">Permissions</span></span>

<span data-ttu-id="6d988-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d988-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d988-108">Permission type</span></span>      | <span data-ttu-id="6d988-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d988-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d988-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d988-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d988-111">監査ログ。 all および All を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d988-111">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="6d988-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d988-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d988-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="6d988-113">Not supported</span></span>   |
|<span data-ttu-id="6d988-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d988-114">Application</span></span> | <span data-ttu-id="6d988-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d988-115">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d988-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d988-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/directoryProvisioning
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d988-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6d988-117">Optional query parameters</span></span>

<span data-ttu-id="6d988-118">このメソッドは、応答をカスタマイズするために、次の OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="6d988-118">This method supports the following OData query parameter to help customize the response.</span></span> <span data-ttu-id="6d988-119">フィルターは、状態を除き、すべて大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="6d988-119">Note that the filters are all case sensitive except for status.</span></span> 

|<span data-ttu-id="6d988-120">名前</span><span class="sxs-lookup"><span data-stu-id="6d988-120">Name</span></span>     |<span data-ttu-id="6d988-121">説明</span><span class="sxs-lookup"><span data-stu-id="6d988-121">Description</span></span>                            |<span data-ttu-id="6d988-122">例</span><span class="sxs-lookup"><span data-stu-id="6d988-122">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="6d988-123">$filter</span><span class="sxs-lookup"><span data-stu-id="6d988-123">$filter</span></span>](/graph/query-parameters#filter-parameter)|<span data-ttu-id="6d988-124">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="6d988-124">Filters results (rows).</span></span> |/`auditLogs/directoryProvisioning?$filter=id eq '74c3b0ae-9cc5-850e-e0a5-7r6a4231de87'`

<span data-ttu-id="6d988-125">一般的な情報については、「 [OData クエリパラメーター](/graph/query_parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d988-125">For general information, see [OData query parameters](/graph/query_parameters).</span></span>

### <a name="attributes-supported-by-the-filter-parameter"></a><span data-ttu-id="6d988-126">$filter パラメーターでサポートされている属性</span><span class="sxs-lookup"><span data-stu-id="6d988-126">Attributes supported by the $filter parameter</span></span>

|<span data-ttu-id="6d988-127">属性名</span><span class="sxs-lookup"><span data-stu-id="6d988-127">Attribute name</span></span> |<span data-ttu-id="6d988-128">サポートされる演算子</span><span class="sxs-lookup"><span data-stu-id="6d988-128">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="6d988-129">id</span><span class="sxs-lookup"><span data-stu-id="6d988-129">id</span></span>| <span data-ttu-id="6d988-130">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-130">eq, contains</span></span>|
|<span data-ttu-id="6d988-131">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="6d988-131">activityDateTime</span></span>| <span data-ttu-id="6d988-132">eq</span><span class="sxs-lookup"><span data-stu-id="6d988-132">eq</span></span>|
|<span data-ttu-id="6d988-133">tenantid</span><span class="sxs-lookup"><span data-stu-id="6d988-133">tenantid</span></span>|<span data-ttu-id="6d988-134">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-134">eq, contains</span></span>|
|<span data-ttu-id="6d988-135">jobid</span><span class="sxs-lookup"><span data-stu-id="6d988-135">jobid</span></span>|<span data-ttu-id="6d988-136">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-136">eq, contains</span></span>|
|<span data-ttu-id="6d988-137">changeid</span><span class="sxs-lookup"><span data-stu-id="6d988-137">changeid</span></span>|<span data-ttu-id="6d988-138">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-138">eq, contains</span></span>|
|<span data-ttu-id="6d988-139">cycleid</span><span class="sxs-lookup"><span data-stu-id="6d988-139">cycleid</span></span>|<span data-ttu-id="6d988-140">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-140">eq, contains</span></span>|
|<span data-ttu-id="6d988-141">action</span><span class="sxs-lookup"><span data-stu-id="6d988-141">action</span></span>|<span data-ttu-id="6d988-142">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-142">eq, contains</span></span>|
|<span data-ttu-id="6d988-143">statusInfo/status</span><span class="sxs-lookup"><span data-stu-id="6d988-143">statusInfo/status</span></span>|<span data-ttu-id="6d988-144">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-144">eq, contains</span></span>|
|<span data-ttu-id="6d988-145">sourceSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="6d988-145">sourceSystem/displayName</span></span>|<span data-ttu-id="6d988-146">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-146">eq, contains</span></span>|
|<span data-ttu-id="6d988-147">targetSystem/displayName</span><span class="sxs-lookup"><span data-stu-id="6d988-147">targetSystem/displayName</span></span>|<span data-ttu-id="6d988-148">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-148">eq, contains</span></span>|
|<span data-ttu-id="6d988-149">sourceIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="6d988-149">sourceIdentity/identityType</span></span>|<span data-ttu-id="6d988-150">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-150">eq, contains</span></span>|
|<span data-ttu-id="6d988-151">targetIdentity/identityType</span><span class="sxs-lookup"><span data-stu-id="6d988-151">targetIdentity/identityType</span></span>|<span data-ttu-id="6d988-152">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-152">eq, contains</span></span>|
|<span data-ttu-id="6d988-153">sourceIdentity/id</span><span class="sxs-lookup"><span data-stu-id="6d988-153">sourceIdentity/id</span></span>|<span data-ttu-id="6d988-154">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-154">eq, contains</span></span>|
|<span data-ttu-id="6d988-155">targetIdentity/id</span><span class="sxs-lookup"><span data-stu-id="6d988-155">targetIdentity/id</span></span>|<span data-ttu-id="6d988-156">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-156">eq, contains</span></span>|
|<span data-ttu-id="6d988-157">sourceIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="6d988-157">sourceIdentity/displayName</span></span>|<span data-ttu-id="6d988-158">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-158">eq, contains</span></span>|
|<span data-ttu-id="6d988-159">targetIdentity/displayName</span><span class="sxs-lookup"><span data-stu-id="6d988-159">targetIdentity/displayName</span></span>|<span data-ttu-id="6d988-160">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-160">eq, contains</span></span>|
|<span data-ttu-id="6d988-161">Initiby/displayName</span><span class="sxs-lookup"><span data-stu-id="6d988-161">initiatedBy/displayName</span></span>|<span data-ttu-id="6d988-162">eq、contains</span><span class="sxs-lookup"><span data-stu-id="6d988-162">eq, contains</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6d988-163">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d988-163">Request headers</span></span>

| <span data-ttu-id="6d988-164">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d988-164">Header</span></span>        | <span data-ttu-id="6d988-165">値</span><span class="sxs-lookup"><span data-stu-id="6d988-165">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="6d988-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d988-166">Authorization</span></span> | <span data-ttu-id="6d988-167">Bearer {トークン} (必須)</span><span class="sxs-lookup"><span data-stu-id="6d988-167">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d988-168">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d988-168">Request body</span></span>

<span data-ttu-id="6d988-169">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6d988-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d988-170">応答</span><span class="sxs-lookup"><span data-stu-id="6d988-170">Response</span></span>

<span data-ttu-id="6d988-171">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、 [provisioningobjectsummary](../resources/provisioningobjectsummary.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6d988-171">If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d988-172">例</span><span class="sxs-lookup"><span data-stu-id="6d988-172">Examples</span></span>

### <a name="example-1-successful-request"></a><span data-ttu-id="6d988-173">例 1: 正常な要求</span><span class="sxs-lookup"><span data-stu-id="6d988-173">Example 1: Successful request</span></span>

### <a name="request"></a><span data-ttu-id="6d988-174">要求</span><span class="sxs-lookup"><span data-stu-id="6d988-174">Request</span></span>

<span data-ttu-id="6d988-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d988-175">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6d988-176">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6d988-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
} -->

```http
GET https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d988-177">C#</span><span class="sxs-lookup"><span data-stu-id="6d988-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d988-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d988-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d988-179">目的-C</span><span class="sxs-lookup"><span data-stu-id="6d988-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d988-180">応答</span><span class="sxs-lookup"><span data-stu-id="6d988-180">Response</span></span>

<span data-ttu-id="6d988-181">成功したイベントに対する応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d988-181">The following is an example of the response for a successful event.</span></span>

><span data-ttu-id="6d988-182">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6d988-182">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d988-183">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d988-183">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryProvisioning",
    "value": [
         {
            "id": "75b5b0ae-9fc5-8d0e-e0a9-7y6a4728de56",
            "activityDateTime": "2019-05-04T03:00:54Z",
            "tenantId": "74beb175-3b80-7b63-b9d5-6f0b76082b16",
            "jobId": "aws.74beb1753b704b63b8d56f0b76082b16.10a7a801-7101-4c69-ae00-ce9f75f8460a",
            "cycleId": "b6502552-018d-79bd-8869-j47194dc65c1",
            "changeId": "b6502552-018d-89bd-9969-b49194dc65c1",
            "action": "EntryExportUpdate",
            "durationInMilliseconds": 3236,
            "statusInfo": {
                "status": "success"
            },
            "provisioningSteps": [
                {
                    "name": "EntryImport",
                    "provisioningStepType": "Import",
                    "status": "success",
                    "description": "Retrieved RolesCompound '10a7a801-7101-4c69-ae00-ce9f75f8460a' from Amazon Web Services",
                    "details": {}
                },
                {
                    "name": "EntryExportUpdate",
                    "provisioningStepType": "Export",
                    "status": "success",
                    "description": "RolesCompound '60a7a801-7101-4c69-ae00-ce9f75f8460a' was updated in Azure Active Directory",
                    "details": {
                        "ReportableIdentifier": "60a7a801-7101-4c69-ae00-ce9f75f8460a"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "appId",
                    "oldValue": null,
                    "newValue": "60a7a801-7101-4c69-ae00-ce9f75f8460a"
                },
                {
                    "displayName": "Roles",
                    "oldValue": null,
                    "newValue": "jaws-prod-role2,jaws-prod-saml2, jayaws-role,jayaws-saml, TestRole,super-saml"
                },
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "6nn37b93-185a-4485-a519-50c09549f3ad"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Amazon Web Services (AWS)"
                },
                {
                    "displayName": "homepage",
                    "oldValue": null,
                    "newValue": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z"
                },
            ],
            "sourceSystem": {
                "id": "d1e090e1-f2f4-4678-be44-6442ffff0621",
                "displayName": "Amazon Web Services",
                "details": {}
            },
            "targetSystem": {
                "id": "e69d4bd2-2da2-483e-bc49-aad4080b91b3",
                "displayName": "Azure Active Directory",
                "details": {
                    "ApplicationId": "bcf4d658-ac9f-408d-bf04-e86dc10328fb",
                    "ServicePrincipalId": "6nn35b93-185a-4485-a519-50c09549f3ad",
                    "ServicePrincipalDisplayName": "Amazon Web Services (AWS)"
                }
            },
            "initiatedBy": {
                "initiatingType": "System",
                "id": "",
                "displayName": "Azure AD Provisioning Service"
            },
            "sourceIdentity": {
                "identityType": "RolesCompound",
                "id": "60a7a801-7101-4c69-ae00-ce9f75f8460a",
                "displayName": "",
                "details": {}
            },
            "targetIdentity": {
                "identityType": "ServicePrincipal",
                "id": "6nn35b93-185a-4485-a519-50c09549f3ad",
                "displayName": "",
                "details": {}
            }
          }
    ]
}

```
### <a name="example-2-error-reponse"></a><span data-ttu-id="6d988-184">例 2: エラー応答</span><span class="sxs-lookup"><span data-stu-id="6d988-184">Example 2: Error reponse</span></span>

### <a name="request"></a><span data-ttu-id="6d988-185">要求</span><span class="sxs-lookup"><span data-stu-id="6d988-185">Request</span></span>

<span data-ttu-id="6d988-186">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d988-186">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6d988-187">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6d988-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary_error"
} -->

```http
GET https://graph.microsoft.com/beta/auditLogs/directoryProvisioning
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d988-188">C#</span><span class="sxs-lookup"><span data-stu-id="6d988-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-provisioningobjectsummary-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d988-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d988-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-provisioningobjectsummary-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d988-190">目的-C</span><span class="sxs-lookup"><span data-stu-id="6d988-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-provisioningobjectsummary-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d988-191">応答</span><span class="sxs-lookup"><span data-stu-id="6d988-191">Response</span></span>

<span data-ttu-id="6d988-192">次に、失敗したプロビジョニングイベントに対する応答の例を示します。</span><span class="sxs-lookup"><span data-stu-id="6d988-192">The following is an example of the response for a failed provisioning event.</span></span>

><span data-ttu-id="6d988-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d988-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary_error"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryProvisioning",
    "value": [
        {
            "id": "gc532ff9-r265-ec76-861e-42e2970a8218",
            "activityDateTime": "2019-06-24T20:53:08Z",
            "tenantId": "7928d5b5-7442-4a97-ne2d-66f9j9972ecn",
            "jobId": "BoxOutDelta.7928d5b574424a97ne2d66f9j9972ecn",
            "cycleId": "44576n58-v14b-70fj-8404-3d22tt46ed93",
            "changeId": "eaad2f8b-e6e3-409b-83bd-e4e2e57177d5",
            "action": "Create",
            "durationInMilliseconds": 2785,
            "sourceSystem": {
                "id": "0404601d-a9c0-4ec7-bbcd-02660120d8c9",
                "displayName": "Azure Active Directory",
                "details": {}
            },
            "targetSystem": {
                "id": "cd22f60b-5f2d-1adg-adb4-76ef31db996b",
                "displayName": "Box",
                "details": {
                    "ApplicationId": "f2764360-e0ec-5676-711e-cd6fc0d4dd61",
                    "ServicePrincipalId": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                    "ServicePrincipalDisplayName": "Box"
                }
            },
            "initiatedBy": {
                "id": "",
                "displayName": "Azure AD Provisioning Service",
                "initiatorType": "system"
            },
            "sourceIdentity": {
                "id": "5e6c9rae-ab4d-5239-8ad0-174391d110eb",
                "displayName": "Self-service Pilot",
                "identityType": "Group",
                "details": {}
            },
            "targetIdentity": {
                "id": "",
                "displayName": "",
                "identityType": "Group",
                "details": {}
            },
            "statusInfo": {
                "@odata.type": "#microsoft.graph.statusDetails",
                "status": "failure",
                "errorCode": "BoxEntryConflict",
                "reason": "Message: Box returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Box via the Box administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Box application in Azure Active Directory or adding a scoping filter to exclude the user.",
                "additionalDetails": null,
                "errorCategory": "NonServiceFailure",
                "recommendedAction": null
            },
            "provisioningSteps": [
                {
                    "name": "EntryImportAdd",
                    "provisioningStepType": "import",
                    "status": "success",
                    "description": "Received Group 'Self-service Pilot' change of type (Add) from Azure Active Directory",
                    "details": {}
                },
                {
                    "name": "EntrySynchronizationAdd",
                    "provisioningStepType": "matching",
                    "status": "success",
                    "description": "Group 'Self-service Pilot' will be created in Box (Group is active and assigned in Azure Active Directory, but no matching Group was found in Box)",
                    "details": {}
                },
                {
                    "name": "EntryExportAdd",
                    "provisioningStepType": "export",
                    "status": "failure",
                    "description": "Failed to create Group 'Self-service Pilot' in Box",
                    "details": {
                        "ReportableIdentifier": "Self-service Pilot"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "5e0c9eae-ad3d-4139-5ad0-174391d110eb"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                },
                {
                    "displayName": "mailEnabled",
                    "oldValue": null,
                    "newValue": "False"
                },
                {
                    "displayName": "mailNickname",
                    "oldValue": null,
                    "newValue": "5ce25n9a-4c5f-45c9-8362-ef3da29c66c5"
                },
                {
                    "displayName": "securityEnabled",
                    "oldValue": null,
                    "newValue": "True"
                },
                {
                    "displayName": "Name",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                }
            ]
       }
    ]
}

```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get provisioningObjectSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
