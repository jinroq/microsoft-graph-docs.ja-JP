---
title: アプリケーションを作成する
description: この API を使用して、新しいアプリケーションを作成します。
localization_priority: Normal
ms.openlocfilehash: 350e5f0fcb45f7404a670c1a0af4e4ddd02a97c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455941"
---
# <a name="create-application"></a><span data-ttu-id="65d44-103">アプリケーションを作成する</span><span class="sxs-lookup"><span data-stu-id="65d44-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65d44-104">この API を使用して、新しいアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="65d44-104">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="65d44-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65d44-105">Permissions</span></span>
<span data-ttu-id="65d44-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65d44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d44-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65d44-108">Permission type</span></span>      | <span data-ttu-id="65d44-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65d44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65d44-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65d44-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65d44-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65d44-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65d44-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65d44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65d44-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65d44-113">Not supported.</span></span>    |
|<span data-ttu-id="65d44-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65d44-114">Application</span></span> | <span data-ttu-id="65d44-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d44-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65d44-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65d44-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="65d44-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65d44-117">Request headers</span></span>
| <span data-ttu-id="65d44-118">名前</span><span class="sxs-lookup"><span data-stu-id="65d44-118">Name</span></span>       | <span data-ttu-id="65d44-119">説明</span><span class="sxs-lookup"><span data-stu-id="65d44-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="65d44-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="65d44-120">Authorization</span></span>  | <span data-ttu-id="65d44-121">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="65d44-121">Bearer.</span></span> <span data-ttu-id="65d44-122">必須</span><span class="sxs-lookup"><span data-stu-id="65d44-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="65d44-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="65d44-123">Request body</span></span>
<span data-ttu-id="65d44-124">要求本文で、 [application](../resources/application.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="65d44-124">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="65d44-125">応答</span><span class="sxs-lookup"><span data-stu-id="65d44-125">Response</span></span>

<span data-ttu-id="65d44-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[application](../resources/application.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65d44-126">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65d44-127">例</span><span class="sxs-lookup"><span data-stu-id="65d44-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65d44-128">要求</span><span class="sxs-lookup"><span data-stu-id="65d44-128">Request</span></span>
<span data-ttu-id="65d44-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65d44-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/{ver}/applications/{id}"
}
```
<span data-ttu-id="65d44-130">要求本文で、 [application](../resources/application.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="65d44-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="65d44-131">応答</span><span class="sxs-lookup"><span data-stu-id="65d44-131">Response</span></span>
<span data-ttu-id="65d44-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65d44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 355

{
  "appId": "appId-value",
  "onPremisesPublishing": {
    "externalUrl": "externalUrl-value",
    "internalUrl": "internalUrl-value",
    "externalAuthenticationType": "externalAuthenticationType-value",
    "customDomainCertificate": "customDomainCertificate-value",
    "isTranslateHostHeaderEnabled": true,
    "isOnPremPublishingEnabled": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-post-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
