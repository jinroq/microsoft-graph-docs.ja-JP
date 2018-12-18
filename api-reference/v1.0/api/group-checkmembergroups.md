---
title: 'グループ: checkMemberGroups'
description: グループの指定されたリスト内のメンバーシップを確認します。 リストから先のグループを返します。
author: dkershaw10
ms.openlocfilehash: 6f31e4f53e99272c456f6bb4263054e9cb5a208f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352494"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="06d02-104">グループ: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="06d02-104">group: checkMemberGroups</span></span>

<span data-ttu-id="06d02-p102">指定したグループ一覧内のメンバーシップを確認します。指定したグループがダイレクト メンバーシップまたは推移性メンバーシップを持つグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="06d02-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="06d02-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="06d02-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="06d02-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="06d02-111">Permissions</span></span>

<span data-ttu-id="06d02-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06d02-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06d02-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06d02-114">Permission type</span></span>                        | <span data-ttu-id="06d02-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="06d02-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="06d02-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06d02-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="06d02-117">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06d02-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="06d02-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06d02-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06d02-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06d02-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="06d02-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06d02-120">Application</span></span>                            | <span data-ttu-id="06d02-121">_Group.Read.All_Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="06d02-121">_Group.Read.All_, Directory.Read.All.</span></span> <span data-ttu-id="06d02-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d02-122">Directory.ReadWrite.All</span></span>                               |

> <span data-ttu-id="06d02-123">**注:** この API は現在必要があります、`Directory.Read.All`アクセス権またはそれ以上です。</span><span class="sxs-lookup"><span data-stu-id="06d02-123">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="06d02-124">使用して、`Group.Read.All`のアクセス許可エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="06d02-124">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="06d02-125">これは既知のバグです。</span><span class="sxs-lookup"><span data-stu-id="06d02-125">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="06d02-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06d02-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="06d02-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06d02-127">Request headers</span></span>

| <span data-ttu-id="06d02-128">名前</span><span class="sxs-lookup"><span data-stu-id="06d02-128">Name</span></span>          | <span data-ttu-id="06d02-129">種類</span><span class="sxs-lookup"><span data-stu-id="06d02-129">Type</span></span>   | <span data-ttu-id="06d02-130">説明</span><span class="sxs-lookup"><span data-stu-id="06d02-130">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="06d02-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="06d02-131">Authorization</span></span> | <span data-ttu-id="06d02-132">string</span><span class="sxs-lookup"><span data-stu-id="06d02-132">string</span></span> | <span data-ttu-id="06d02-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="06d02-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06d02-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="06d02-135">Request body</span></span>

<span data-ttu-id="06d02-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="06d02-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06d02-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="06d02-137">Parameter</span></span> | <span data-ttu-id="06d02-138">種類</span><span class="sxs-lookup"><span data-stu-id="06d02-138">Type</span></span>              | <span data-ttu-id="06d02-139">説明</span><span class="sxs-lookup"><span data-stu-id="06d02-139">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="06d02-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="06d02-140">groupIds</span></span>  | <span data-ttu-id="06d02-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="06d02-141">String collection</span></span> | <span data-ttu-id="06d02-142">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="06d02-142">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="06d02-143">応答</span><span class="sxs-lookup"><span data-stu-id="06d02-143">Response</span></span>

<span data-ttu-id="06d02-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="06d02-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06d02-145">例</span><span class="sxs-lookup"><span data-stu-id="06d02-145">Example</span></span>

<span data-ttu-id="06d02-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="06d02-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="06d02-147">要求</span><span class="sxs-lookup"><span data-stu-id="06d02-147">Request</span></span>

<span data-ttu-id="06d02-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="06d02-148">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="06d02-149">応答</span><span class="sxs-lookup"><span data-stu-id="06d02-149">Response</span></span>

<span data-ttu-id="06d02-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="06d02-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
