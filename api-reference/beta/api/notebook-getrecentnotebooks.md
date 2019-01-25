---
title: 'ノートブック: getRecentNotebooks'
description: サインインしたユーザーによってアクセスされた recentNotebook インスタンスの一覧を取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 90f620a82794bb575d9dfa35f2ad31b062b2faf4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527704"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="3ad8e-103">ノートブック: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="3ad8e-103">notebook: getRecentNotebooks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ad8e-104">サインインしたユーザーによってアクセスされた [recentNotebook](../resources/recentnotebook.md) インスタンスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ad8e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3ad8e-105">Permissions</span></span>
<span data-ttu-id="3ad8e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ad8e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ad8e-108">Permission type</span></span>      | <span data-ttu-id="3ad8e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ad8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ad8e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ad8e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ad8e-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All、</span><span class="sxs-lookup"><span data-stu-id="3ad8e-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="3ad8e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ad8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ad8e-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ad8e-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="3ad8e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ad8e-114">Application</span></span> | <span data-ttu-id="3ad8e-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ad8e-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ad8e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ad8e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="3ad8e-117">ユーザーの `<id | userPrincipalName>` は、要求を行うために使用された承認トークンにおいてエンコードされたユーザーと一致しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-117">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="3ad8e-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="3ad8e-118">Function parameters</span></span>

| <span data-ttu-id="3ad8e-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3ad8e-119">Parameter</span></span>    | <span data-ttu-id="3ad8e-120">型</span><span class="sxs-lookup"><span data-stu-id="3ad8e-120">Type</span></span>   |<span data-ttu-id="3ad8e-121">説明</span><span class="sxs-lookup"><span data-stu-id="3ad8e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ad8e-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="3ad8e-122">includePersonalNotebooks</span></span>|<span data-ttu-id="3ad8e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ad8e-123">Boolean</span></span>|<span data-ttu-id="3ad8e-124">ユーザーが所有しているノートブックを含みます。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="3ad8e-125">ユーザーが所有しているノートブックを含むには、`true` に設定します。そうでない場合は、`false` に設定します。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="3ad8e-126">`includePersonalNotebooks` パラメーターを含めない場合、要求は `400` エラー応答を返します。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3ad8e-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ad8e-127">Request headers</span></span>
| <span data-ttu-id="3ad8e-128">名前</span><span class="sxs-lookup"><span data-stu-id="3ad8e-128">Name</span></span>       | <span data-ttu-id="3ad8e-129">説明</span><span class="sxs-lookup"><span data-stu-id="3ad8e-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ad8e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ad8e-130">Authorization</span></span>  | <span data-ttu-id="3ad8e-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3ad8e-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ad8e-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ad8e-132">Request body</span></span>
<span data-ttu-id="3ad8e-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ad8e-134">応答</span><span class="sxs-lookup"><span data-stu-id="3ad8e-134">Response</span></span>
<span data-ttu-id="3ad8e-135">正常な応答は **recentNotebooks** の JSON コレクションを含む `200 OK` を返します。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="3ad8e-136">例</span><span class="sxs-lookup"><span data-stu-id="3ad8e-136">Example</span></span>
<span data-ttu-id="3ad8e-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3ad8e-138">要求</span><span class="sxs-lookup"><span data-stu-id="3ad8e-138">Request</span></span>
<span data-ttu-id="3ad8e-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-139">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="3ad8e-140">応答</span><span class="sxs-lookup"><span data-stu-id="3ad8e-140">Response</span></span>
<span data-ttu-id="3ad8e-141">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="3ad8e-141">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-getrecentnotebooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
