---
title: Outlooktaskfolder を更新します。
description: Outlook の仕事フォルダーの書き込み可能なプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 83b75fb2588f58480e51e4e548bfd5d05b7f941b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530161"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="7dda4-103">Outlooktaskfolder を更新します。</span><span class="sxs-lookup"><span data-stu-id="7dda4-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dda4-104">Outlook の仕事フォルダーの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7dda4-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="7dda4-105">既定の作業フォルダーのタスク」の**name**プロパティの値を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="7dda4-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="7dda4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7dda4-106">Permissions</span></span>
<span data-ttu-id="7dda4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7dda4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dda4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7dda4-109">Permission type</span></span>      | <span data-ttu-id="7dda4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7dda4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dda4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7dda4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7dda4-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dda4-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7dda4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7dda4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dda4-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dda4-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7dda4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7dda4-115">Application</span></span> | <span data-ttu-id="7dda4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dda4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dda4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7dda4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7dda4-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dda4-118">Optional request headers</span></span>
| <span data-ttu-id="7dda4-119">名前</span><span class="sxs-lookup"><span data-stu-id="7dda4-119">Name</span></span>       | <span data-ttu-id="7dda4-120">説明</span><span class="sxs-lookup"><span data-stu-id="7dda4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7dda4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dda4-121">Authorization</span></span>  | <span data-ttu-id="7dda4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7dda4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dda4-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="7dda4-124">Request body</span></span>
<span data-ttu-id="7dda4-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7dda4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7dda4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dda4-128">Property</span></span>     | <span data-ttu-id="7dda4-129">型</span><span class="sxs-lookup"><span data-stu-id="7dda4-129">Type</span></span>   |<span data-ttu-id="7dda4-130">説明</span><span class="sxs-lookup"><span data-stu-id="7dda4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7dda4-131">name</span><span class="sxs-lookup"><span data-stu-id="7dda4-131">name</span></span>|<span data-ttu-id="7dda4-132">String</span><span class="sxs-lookup"><span data-stu-id="7dda4-132">String</span></span>|<span data-ttu-id="7dda4-133">タスク フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="7dda4-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="7dda4-134">応答</span><span class="sxs-lookup"><span data-stu-id="7dda4-134">Response</span></span>

<span data-ttu-id="7dda4-135">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[outlookTaskFolder](../resources/outlooktaskfolder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7dda4-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7dda4-136">例</span><span class="sxs-lookup"><span data-stu-id="7dda4-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7dda4-137">要求</span><span class="sxs-lookup"><span data-stu-id="7dda4-137">Request</span></span>
<span data-ttu-id="7dda4-138">次の例に指定したタスク フォルダーの名前を変更する`Charity work`。</span><span class="sxs-lookup"><span data-stu-id="7dda4-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>
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
##### <a name="response"></a><span data-ttu-id="7dda4-139">応答</span><span class="sxs-lookup"><span data-stu-id="7dda4-139">Response</span></span>
<span data-ttu-id="7dda4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7dda4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
