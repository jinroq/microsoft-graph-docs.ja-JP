---
title: リスト directorySettingTemplates
description: テンプレートを設定するディレクトリは、ディレクトリの設定、どのディレクトリから設定を作成し、テナント内で使用されるテンプレートのセットを表します。  この操作は、使用可能な directorySettingTemplates オブジェクトの一覧を取得します。
ms.openlocfilehash: 964e2cfc9e06b6a996f63c92cae830e03c953cd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071042"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="2bb2b-104">リスト directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="2bb2b-104">List directorySettingTemplates</span></span>

> <span data-ttu-id="2bb2b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bb2b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bb2b-107">テンプレートを設定するディレクトリは、ディレクトリの設定、どのディレクトリから設定を作成し、テナント内で使用されるテンプレートのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-107">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="2bb2b-108">この操作は、使用可能な directorySettingTemplates オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-108">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="2bb2b-109">**注**: この API の/beta バージョンは、のみのグループに適用されます。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="2bb2b-110">この API の/v1.0 のバージョンは*groupSettingTemplate のリスト*に名前変更されました。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-110">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bb2b-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2bb2b-111">Permissions</span></span>
<span data-ttu-id="2bb2b-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bb2b-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2bb2b-114">Permission type</span></span>      | <span data-ttu-id="2bb2b-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2bb2b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bb2b-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2bb2b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="2bb2b-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2bb2b-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2bb2b-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2bb2b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bb2b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-119">Not supported.</span></span>    |
|<span data-ttu-id="2bb2b-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2bb2b-120">Application</span></span> | <span data-ttu-id="2bb2b-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bb2b-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bb2b-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2bb2b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2bb2b-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2bb2b-123">Optional query parameters</span></span>
<span data-ttu-id="2bb2b-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bb2b-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bb2b-125">Request headers</span></span>
| <span data-ttu-id="2bb2b-126">名前</span><span class="sxs-lookup"><span data-stu-id="2bb2b-126">Name</span></span>      |<span data-ttu-id="2bb2b-127">説明</span><span class="sxs-lookup"><span data-stu-id="2bb2b-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2bb2b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bb2b-128">Authorization</span></span>  | <span data-ttu-id="2bb2b-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bb2b-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="2bb2b-131">Request body</span></span>
<span data-ttu-id="2bb2b-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bb2b-133">応答</span><span class="sxs-lookup"><span data-stu-id="2bb2b-133">Response</span></span>

<span data-ttu-id="2bb2b-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[directorySettingTemplate](../resources/directorysettingtemplate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-134">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2bb2b-135">例</span><span class="sxs-lookup"><span data-stu-id="2bb2b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bb2b-136">要求</span><span class="sxs-lookup"><span data-stu-id="2bb2b-136">Request</span></span>
<span data-ttu-id="2bb2b-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="2bb2b-138">応答</span><span class="sxs-lookup"><span data-stu-id="2bb2b-138">Response</span></span>
<span data-ttu-id="2bb2b-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2bb2b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
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
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->