---
title: ディレクトリの設定を一覧表示する
description: ディレクトリ設定オブジェクトの一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 708faad9dc90bf5f79f89d72b381391843371766
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454828"
---
# <a name="list-directory-settings"></a><span data-ttu-id="6a26a-103">ディレクトリの設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6a26a-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a26a-104">ディレクトリ設定オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a26a-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="6a26a-105">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6a26a-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="6a26a-106">この API の/v1.0 バージョンは、[ *groupsettings]* の名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="6a26a-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a26a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a26a-107">Permissions</span></span>
<span data-ttu-id="6a26a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a26a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a26a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a26a-110">Permission type</span></span>      | <span data-ttu-id="6a26a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a26a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a26a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a26a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a26a-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a26a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a26a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a26a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a26a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a26a-115">Not supported.</span></span>    |
|<span data-ttu-id="6a26a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a26a-116">Application</span></span> | <span data-ttu-id="6a26a-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a26a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a26a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a26a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6a26a-119">テナント全体またはグループ設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6a26a-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a26a-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6a26a-120">Optional query parameters</span></span>
<span data-ttu-id="6a26a-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6a26a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a26a-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a26a-122">Request headers</span></span>
| <span data-ttu-id="6a26a-123">名前</span><span class="sxs-lookup"><span data-stu-id="6a26a-123">Name</span></span>      |<span data-ttu-id="6a26a-124">説明</span><span class="sxs-lookup"><span data-stu-id="6a26a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a26a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a26a-125">Authorization</span></span>  | <span data-ttu-id="6a26a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a26a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a26a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a26a-128">Request body</span></span>
<span data-ttu-id="6a26a-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6a26a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a26a-130">応答</span><span class="sxs-lookup"><span data-stu-id="6a26a-130">Response</span></span>

<span data-ttu-id="6a26a-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[directorysetting](../resources/directorysetting.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6a26a-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a26a-132">例</span><span class="sxs-lookup"><span data-stu-id="6a26a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a26a-133">要求</span><span class="sxs-lookup"><span data-stu-id="6a26a-133">Request</span></span>
<span data-ttu-id="6a26a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a26a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="6a26a-135">応答</span><span class="sxs-lookup"><span data-stu-id="6a26a-135">Response</span></span>
<span data-ttu-id="6a26a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a26a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "settingTemplateId": "settingTemplateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
