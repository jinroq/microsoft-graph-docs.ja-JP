---
title: Outlooktaskfolder を更新します。
description: Outlook の仕事フォルダーの書き込み可能なプロパティを更新します。
author: angelgolfer-ms
ms.openlocfilehash: 83b78a7d3ff625a6eaaacd3ac54612e487350cde
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313973"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="44d1e-103">Outlooktaskfolder を更新します。</span><span class="sxs-lookup"><span data-stu-id="44d1e-103">Update outlooktaskfolder</span></span>

> <span data-ttu-id="44d1e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44d1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44d1e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44d1e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44d1e-106">Outlook の仕事フォルダーの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="44d1e-106">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="44d1e-107">既定の作業フォルダーのタスク」の**name**プロパティの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="44d1e-107">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="44d1e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44d1e-108">Permissions</span></span>
<span data-ttu-id="44d1e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44d1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44d1e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44d1e-111">Permission type</span></span>      | <span data-ttu-id="44d1e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44d1e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44d1e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44d1e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="44d1e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44d1e-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="44d1e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44d1e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44d1e-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44d1e-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="44d1e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44d1e-117">Application</span></span> | <span data-ttu-id="44d1e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44d1e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44d1e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44d1e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="44d1e-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44d1e-120">Optional request headers</span></span>
| <span data-ttu-id="44d1e-121">名前</span><span class="sxs-lookup"><span data-stu-id="44d1e-121">Name</span></span>       | <span data-ttu-id="44d1e-122">説明</span><span class="sxs-lookup"><span data-stu-id="44d1e-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="44d1e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44d1e-123">Authorization</span></span>  | <span data-ttu-id="44d1e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44d1e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44d1e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="44d1e-126">Request body</span></span>
<span data-ttu-id="44d1e-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="44d1e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="44d1e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44d1e-130">Property</span></span>     | <span data-ttu-id="44d1e-131">種類</span><span class="sxs-lookup"><span data-stu-id="44d1e-131">Type</span></span>   |<span data-ttu-id="44d1e-132">説明</span><span class="sxs-lookup"><span data-stu-id="44d1e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44d1e-133">名前</span><span class="sxs-lookup"><span data-stu-id="44d1e-133">name</span></span>|<span data-ttu-id="44d1e-134">String</span><span class="sxs-lookup"><span data-stu-id="44d1e-134">String</span></span>|<span data-ttu-id="44d1e-135">タスク フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="44d1e-135">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="44d1e-136">応答</span><span class="sxs-lookup"><span data-stu-id="44d1e-136">Response</span></span>

<span data-ttu-id="44d1e-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[outlookTaskFolder](../resources/outlooktaskfolder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="44d1e-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44d1e-138">例</span><span class="sxs-lookup"><span data-stu-id="44d1e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44d1e-139">要求</span><span class="sxs-lookup"><span data-stu-id="44d1e-139">Request</span></span>
<span data-ttu-id="44d1e-140">次の例に指定したタスク フォルダーの名前を変更する`Charity work`。</span><span class="sxs-lookup"><span data-stu-id="44d1e-140">The following example changes the name of the specified task folder to `Charity work`.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPWAAA=')
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
##### <a name="response"></a><span data-ttu-id="44d1e-141">応答</span><span class="sxs-lookup"><span data-stu-id="44d1e-141">Response</span></span>
<span data-ttu-id="44d1e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44d1e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAKfQ==",
  "isDefaultFolder": false,
  "name": "Charity work",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->