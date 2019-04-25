---
title: 同期テンプレートを取得する
description: その識別子で同期テンプレートを取得します。
localization_priority: Normal
ms.openlocfilehash: 4fc13ee5d83d6501f75bb45ce69f189b8809270c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545172"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="28c41-103">同期テンプレートを取得する</span><span class="sxs-lookup"><span data-stu-id="28c41-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28c41-104">その識別子で同期テンプレートを取得します。</span><span class="sxs-lookup"><span data-stu-id="28c41-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="28c41-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="28c41-105">Permissions</span></span>
<span data-ttu-id="28c41-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28c41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c41-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28c41-108">Permission type</span></span>                        | <span data-ttu-id="28c41-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="28c41-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="28c41-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28c41-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="28c41-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c41-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="28c41-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28c41-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="28c41-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28c41-113">Not supported.</span></span>|
|<span data-ttu-id="28c41-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28c41-114">Application</span></span>                            |<span data-ttu-id="28c41-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28c41-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="28c41-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28c41-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="28c41-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28c41-117">Request headers</span></span>

| <span data-ttu-id="28c41-118">名前</span><span class="sxs-lookup"><span data-stu-id="28c41-118">Name</span></span>           | <span data-ttu-id="28c41-119">型</span><span class="sxs-lookup"><span data-stu-id="28c41-119">Type</span></span>    | <span data-ttu-id="28c41-120">説明</span><span class="sxs-lookup"><span data-stu-id="28c41-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="28c41-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28c41-121">Authorization</span></span>  | <span data-ttu-id="28c41-122">string</span><span class="sxs-lookup"><span data-stu-id="28c41-122">string</span></span>  | <span data-ttu-id="28c41-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="28c41-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28c41-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="28c41-125">Request body</span></span>

<span data-ttu-id="28c41-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="28c41-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="28c41-127">応答</span><span class="sxs-lookup"><span data-stu-id="28c41-127">Response</span></span>

<span data-ttu-id="28c41-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="28c41-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="28c41-129">例</span><span class="sxs-lookup"><span data-stu-id="28c41-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="28c41-130">要求</span><span class="sxs-lookup"><span data-stu-id="28c41-130">Request</span></span>
<span data-ttu-id="28c41-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="28c41-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="28c41-132">応答</span><span class="sxs-lookup"><span data-stu-id="28c41-132">Response</span></span>
<span data-ttu-id="28c41-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="28c41-133">The following is an example of a response.</span></span>
><span data-ttu-id="28c41-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="28c41-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="28c41-135">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="28c41-135">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
