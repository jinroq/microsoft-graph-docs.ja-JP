---
title: ディレクトリ設定のテンプレートを取得します。
description: ディレクトリ設定のテンプレートでは、テナント内で元の設定を作成する可能性があります設定のテンプレートを表します。 この操作には、使用可能な設定とその既定値を含む directorySettingTemplate オブジェクトのプロパティの取得が可能します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2fb9f8edbc374760f16496bd9ec5bcf666a09883
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935676"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="4faff-104">ディレクトリ設定のテンプレートを取得します。</span><span class="sxs-lookup"><span data-stu-id="4faff-104">Get a directory setting template</span></span>

> <span data-ttu-id="4faff-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4faff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4faff-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4faff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4faff-107">ディレクトリ設定のテンプレートでは、テナント内で元の設定を作成する可能性があります設定のテンプレートを表します。</span><span class="sxs-lookup"><span data-stu-id="4faff-107">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="4faff-108">この操作には、使用可能な設定とその既定値を含む directorySettingTemplate オブジェクトのプロパティの取得が可能します。</span><span class="sxs-lookup"><span data-stu-id="4faff-108">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="4faff-109">**注**: この API の/beta バージョンは、のみのグループに適用されます。</span><span class="sxs-lookup"><span data-stu-id="4faff-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="4faff-110">この API の/v1.0 バージョンの名前は*groupSettingTemplate を取得*します。</span><span class="sxs-lookup"><span data-stu-id="4faff-110">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="4faff-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4faff-111">Permissions</span></span>
<span data-ttu-id="4faff-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4faff-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4faff-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4faff-114">Permission type</span></span>      | <span data-ttu-id="4faff-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4faff-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4faff-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4faff-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4faff-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4faff-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4faff-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4faff-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4faff-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4faff-119">Not supported.</span></span>    |
|<span data-ttu-id="4faff-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4faff-120">Application</span></span> | <span data-ttu-id="4faff-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4faff-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4faff-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4faff-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4faff-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4faff-123">Optional query parameters</span></span>
<span data-ttu-id="4faff-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4faff-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4faff-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4faff-125">Request headers</span></span>
| <span data-ttu-id="4faff-126">名前</span><span class="sxs-lookup"><span data-stu-id="4faff-126">Name</span></span>      |<span data-ttu-id="4faff-127">説明</span><span class="sxs-lookup"><span data-stu-id="4faff-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4faff-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="4faff-128">Authorization</span></span>  | <span data-ttu-id="4faff-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4faff-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4faff-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="4faff-131">Request body</span></span>
<span data-ttu-id="4faff-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4faff-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4faff-133">応答</span><span class="sxs-lookup"><span data-stu-id="4faff-133">Response</span></span>

<span data-ttu-id="4faff-134">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[directorySettingTemplate](../resources/directorysettingtemplate.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4faff-134">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4faff-135">例</span><span class="sxs-lookup"><span data-stu-id="4faff-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4faff-136">要求</span><span class="sxs-lookup"><span data-stu-id="4faff-136">Request</span></span>
<span data-ttu-id="4faff-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4faff-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="4faff-138">応答</span><span class="sxs-lookup"><span data-stu-id="4faff-138">Response</span></span>
<span data-ttu-id="4faff-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4faff-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
