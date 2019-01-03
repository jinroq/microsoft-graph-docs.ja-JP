---
title: 'ノートブック: getRecentNotebooks'
description: サインインしたユーザーによってアクセスされた recentNotebook インスタンスの一覧を取得します。
author: Jewan-microsoft
ms.openlocfilehash: 43141d7734a3427a3325a852d8185ebbee5d752c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350499"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="36c6d-103">ノートブック: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="36c6d-103">notebook: getRecentNotebooks</span></span>

> <span data-ttu-id="36c6d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="36c6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36c6d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36c6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36c6d-106">サインインしたユーザーによってアクセスされた [recentNotebook](../resources/recentnotebook.md) インスタンスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="36c6d-106">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="36c6d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36c6d-107">Permissions</span></span>
<span data-ttu-id="36c6d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36c6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c6d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36c6d-110">Permission type</span></span>      | <span data-ttu-id="36c6d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36c6d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36c6d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36c6d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="36c6d-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All、</span><span class="sxs-lookup"><span data-stu-id="36c6d-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="36c6d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36c6d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36c6d-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36c6d-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="36c6d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36c6d-116">Application</span></span> | <span data-ttu-id="36c6d-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c6d-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36c6d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36c6d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="36c6d-119">ユーザーの `<id | userPrincipalName>` は、要求を行うために使用された承認トークンにおいてエンコードされたユーザーと一致しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="36c6d-119">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="36c6d-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="36c6d-120">Function parameters</span></span>

| <span data-ttu-id="36c6d-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="36c6d-121">Parameter</span></span>    | <span data-ttu-id="36c6d-122">種類</span><span class="sxs-lookup"><span data-stu-id="36c6d-122">Type</span></span>   |<span data-ttu-id="36c6d-123">説明</span><span class="sxs-lookup"><span data-stu-id="36c6d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36c6d-124">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="36c6d-124">includePersonalNotebooks</span></span>|<span data-ttu-id="36c6d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="36c6d-125">Boolean</span></span>|<span data-ttu-id="36c6d-126">ユーザーが所有しているノートブックを含みます。</span><span class="sxs-lookup"><span data-stu-id="36c6d-126">Include notebooks owned by the user.</span></span> <span data-ttu-id="36c6d-127">ユーザーが所有しているノートブックを含むには、`true` に設定します。そうでない場合は、`false` に設定します。</span><span class="sxs-lookup"><span data-stu-id="36c6d-127">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="36c6d-128">`includePersonalNotebooks` パラメーターを含めない場合、要求は `400` エラー応答を返します。</span><span class="sxs-lookup"><span data-stu-id="36c6d-128">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="36c6d-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36c6d-129">Request headers</span></span>
| <span data-ttu-id="36c6d-130">名前</span><span class="sxs-lookup"><span data-stu-id="36c6d-130">Name</span></span>       | <span data-ttu-id="36c6d-131">説明</span><span class="sxs-lookup"><span data-stu-id="36c6d-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36c6d-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="36c6d-132">Authorization</span></span>  | <span data-ttu-id="36c6d-133">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="36c6d-133">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="36c6d-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="36c6d-134">Request body</span></span>
<span data-ttu-id="36c6d-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="36c6d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36c6d-136">応答</span><span class="sxs-lookup"><span data-stu-id="36c6d-136">Response</span></span>
<span data-ttu-id="36c6d-137">正常な応答は **recentNotebooks** の JSON コレクションを含む `200 OK` を返します。</span><span class="sxs-lookup"><span data-stu-id="36c6d-137">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="36c6d-138">例</span><span class="sxs-lookup"><span data-stu-id="36c6d-138">Example</span></span>
<span data-ttu-id="36c6d-139">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="36c6d-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="36c6d-140">要求</span><span class="sxs-lookup"><span data-stu-id="36c6d-140">Request</span></span>
<span data-ttu-id="36c6d-141">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="36c6d-141">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="36c6d-142">応答</span><span class="sxs-lookup"><span data-stu-id="36c6d-142">Response</span></span>
<span data-ttu-id="36c6d-143">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="36c6d-143">The following example shows the response.</span></span>

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