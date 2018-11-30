---
title: セッションを作成する
description: 'この API を使用して、新しいブック セッションを作成します。 '
ms.openlocfilehash: 912574850c725c021f630e68fbe12d333f146593
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074042"
---
# <a name="create-session"></a><span data-ttu-id="6b492-103">セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="6b492-103">Create Session</span></span>

<span data-ttu-id="6b492-104">この API を使用して、新しいブック セッションを作成します。</span><span class="sxs-lookup"><span data-stu-id="6b492-104">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="6b492-105">2 つのモードのいずれかで、Excel API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="6b492-105">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="6b492-p101">永続セッション - ブックに加えられたすべての変更は永続化 (保存) されます。これは通常の操作モードです。</span><span class="sxs-lookup"><span data-stu-id="6b492-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="6b492-p102">非永続セッション - API によって加えられた変更は元の場所に保存されません。代わりに、その特定の API セッション中に加えられた変更を反映するファイルの一時コピーが Excel のバックエンド サーバーに保持されます。Excel のセッションの有効期限が切れると、変更は失われます。分析を行ったり、計算の結果やグラフのイメージを取得したりする必要があるものの、ドキュメントの状態には影響を与えないアプリには、このモードが便利です。</span><span class="sxs-lookup"><span data-stu-id="6b492-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="6b492-112">API でセッションを表すには、`workbook-session-id: {session-id}` ヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="6b492-112">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="6b492-p103">**注:** セッション ヘッダーは Excel API が機能するために必要ではありません。しかし、パフォーマンスを向上させるためにセッション ヘッダーを使用することをお勧めします。セッション ヘッダーを使用しない場合は、API の呼び出し時に行われた変更がファイルに永続化_されます_。</span><span class="sxs-lookup"><span data-stu-id="6b492-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="error-handling"></a><span data-ttu-id="6b492-116">エラー処理</span><span class="sxs-lookup"><span data-stu-id="6b492-116">Error Handling</span></span>

<span data-ttu-id="6b492-117">この要求に対して、504 HTTP エラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6b492-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="6b492-118">このエラーに対する適切な対応は、要求を繰り返すことです。</span><span class="sxs-lookup"><span data-stu-id="6b492-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b492-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6b492-119">Permissions</span></span>
<span data-ttu-id="6b492-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b492-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b492-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b492-122">Permission type</span></span>      | <span data-ttu-id="6b492-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b492-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b492-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b492-124">Delegated (work or school account)</span></span> | <span data-ttu-id="6b492-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b492-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b492-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b492-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b492-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b492-127">Not supported.</span></span>    |
|<span data-ttu-id="6b492-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b492-128">Application</span></span> | <span data-ttu-id="6b492-129">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b492-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b492-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b492-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="6b492-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b492-131">Request headers</span></span>
| <span data-ttu-id="6b492-132">名前</span><span class="sxs-lookup"><span data-stu-id="6b492-132">Name</span></span>       | <span data-ttu-id="6b492-133">説明</span><span class="sxs-lookup"><span data-stu-id="6b492-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6b492-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b492-134">Authorization</span></span>  | <span data-ttu-id="6b492-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6b492-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b492-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b492-137">Request body</span></span>
<span data-ttu-id="6b492-138">要求本文で、[WorkbookSessionInfo](../resources/workbooksessioninfo.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b492-138">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6b492-139">応答</span><span class="sxs-lookup"><span data-stu-id="6b492-139">Response</span></span>

<span data-ttu-id="6b492-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [WorkbookSessionInfo](../resources/workbooksessioninfo.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6b492-140">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b492-141">例</span><span class="sxs-lookup"><span data-stu-id="6b492-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b492-142">要求</span><span class="sxs-lookup"><span data-stu-id="6b492-142">Request</span></span>
<span data-ttu-id="6b492-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b492-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistSession": true
}
```
<span data-ttu-id="6b492-144">要求本文で、[WorkbookSessionInfo](../resources/workbooksessioninfo.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b492-144">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="6b492-145">応答</span><span class="sxs-lookup"><span data-stu-id="6b492-145">Response</span></span>
<span data-ttu-id="6b492-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6b492-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistSession": true
}
```

