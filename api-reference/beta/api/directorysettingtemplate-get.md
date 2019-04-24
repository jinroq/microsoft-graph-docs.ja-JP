---
title: ディレクトリ設定テンプレートを取得する
description: ディレクトリ設定テンプレートは、テナント内で設定を作成することができる設定のテンプレートを表します。 この操作により、使用可能な設定とその既定値を含む directorysettingtemplate オブジェクトのプロパティを取得できるようになります。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c097d9919a52cde8559ead338f433b27a1e3e73d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454940"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="c3301-104">ディレクトリ設定テンプレートを取得する</span><span class="sxs-lookup"><span data-stu-id="c3301-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3301-105">ディレクトリ設定テンプレートは、テナント内で設定を作成することができる設定のテンプレートを表します。</span><span class="sxs-lookup"><span data-stu-id="c3301-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="c3301-106">この操作により、使用可能な設定とその既定値を含む directorysettingtemplate オブジェクトのプロパティを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="c3301-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="c3301-107">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="c3301-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="c3301-108">この API の/v1.0 バージョンは、 *groupsettingtemplate を取得*する名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="c3301-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3301-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3301-109">Permissions</span></span>
<span data-ttu-id="c3301-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3301-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3301-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3301-112">Permission type</span></span>      | <span data-ttu-id="c3301-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3301-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3301-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3301-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c3301-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3301-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c3301-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3301-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3301-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3301-117">Not supported.</span></span>    |
|<span data-ttu-id="c3301-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3301-118">Application</span></span> | <span data-ttu-id="c3301-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3301-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3301-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3301-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3301-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3301-121">Optional query parameters</span></span>
<span data-ttu-id="c3301-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c3301-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3301-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3301-123">Request headers</span></span>
| <span data-ttu-id="c3301-124">名前</span><span class="sxs-lookup"><span data-stu-id="c3301-124">Name</span></span>      |<span data-ttu-id="c3301-125">説明</span><span class="sxs-lookup"><span data-stu-id="c3301-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3301-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3301-126">Authorization</span></span>  | <span data-ttu-id="c3301-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3301-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3301-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3301-129">Request body</span></span>
<span data-ttu-id="c3301-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3301-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3301-131">応答</span><span class="sxs-lookup"><span data-stu-id="c3301-131">Response</span></span>

<span data-ttu-id="c3301-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[directorysettingtemplate](../resources/directorysettingtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3301-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3301-133">例</span><span class="sxs-lookup"><span data-stu-id="c3301-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3301-134">要求</span><span class="sxs-lookup"><span data-stu-id="c3301-134">Request</span></span>
<span data-ttu-id="c3301-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3301-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="c3301-136">応答</span><span class="sxs-lookup"><span data-stu-id="c3301-136">Response</span></span>
<span data-ttu-id="c3301-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3301-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 270

{
  "id": "id-value",
  "displayName": "displayName-value",
  "description": "description-value",
  "values": [
    {
      "name": "name-value",
      "type": "type-value",
      "defaultValue": "defaultValue-value",
      "description": "description-value"
    }
  ],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
