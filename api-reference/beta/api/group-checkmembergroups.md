---
title: 'グループ: checkMemberGroups'
description: 指定したグループ一覧内のメンバーシップを確認します。 対象となるグループのリストからを返します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 838ea805f6732965029690a05e8d3294fdd62c26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503109"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="95fae-104">グループ: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="95fae-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95fae-p102">指定したグループ一覧内のメンバーシップを確認します。指定したグループがダイレクト メンバーシップまたは推移性メンバーシップを持つグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="95fae-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="95fae-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="95fae-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="95fae-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="95fae-111">Permissions</span></span>

<span data-ttu-id="95fae-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95fae-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95fae-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95fae-114">Permission type</span></span>                        | <span data-ttu-id="95fae-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="95fae-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="95fae-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95fae-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="95fae-117">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95fae-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="95fae-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95fae-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95fae-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95fae-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="95fae-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95fae-120">Application</span></span>                            | <span data-ttu-id="95fae-121">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95fae-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="95fae-122">**注:** この API には、 `Directory.Read.All`現在アクセス許可以上が必要です。</span><span class="sxs-lookup"><span data-stu-id="95fae-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="95fae-123">`Group.Read.All`アクセス許可を使用すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="95fae-123">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="95fae-124">これは既知のバグです。</span><span class="sxs-lookup"><span data-stu-id="95fae-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="95fae-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95fae-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="95fae-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95fae-126">Request headers</span></span>

| <span data-ttu-id="95fae-127">名前</span><span class="sxs-lookup"><span data-stu-id="95fae-127">Name</span></span>          | <span data-ttu-id="95fae-128">型</span><span class="sxs-lookup"><span data-stu-id="95fae-128">Type</span></span>   | <span data-ttu-id="95fae-129">説明</span><span class="sxs-lookup"><span data-stu-id="95fae-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="95fae-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="95fae-130">Authorization</span></span> | <span data-ttu-id="95fae-131">string</span><span class="sxs-lookup"><span data-stu-id="95fae-131">string</span></span> | <span data-ttu-id="95fae-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="95fae-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95fae-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="95fae-134">Request body</span></span>

<span data-ttu-id="95fae-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="95fae-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="95fae-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="95fae-136">Parameter</span></span> | <span data-ttu-id="95fae-137">型</span><span class="sxs-lookup"><span data-stu-id="95fae-137">Type</span></span>   | <span data-ttu-id="95fae-138">説明</span><span class="sxs-lookup"><span data-stu-id="95fae-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="95fae-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="95fae-139">groupIds</span></span>  | <span data-ttu-id="95fae-140">String</span><span class="sxs-lookup"><span data-stu-id="95fae-140">String</span></span> | <span data-ttu-id="95fae-141">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="95fae-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="95fae-142">応答</span><span class="sxs-lookup"><span data-stu-id="95fae-142">Response</span></span>

<span data-ttu-id="95fae-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95fae-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95fae-144">例</span><span class="sxs-lookup"><span data-stu-id="95fae-144">Example</span></span>

<span data-ttu-id="95fae-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="95fae-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="95fae-146">要求</span><span class="sxs-lookup"><span data-stu-id="95fae-146">Request</span></span>

<span data-ttu-id="95fae-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95fae-147">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="95fae-148">応答</span><span class="sxs-lookup"><span data-stu-id="95fae-148">Response</span></span>

<span data-ttu-id="95fae-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95fae-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
