---
title: グループを更新する
description: '[グループ](../resources/group.md)オブジェクトのプロパティを更新します。'
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dc98862027c48e9615e3d57b07a1f87c05b8c272
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442686"
---
# <a name="update-group"></a><span data-ttu-id="2b1e6-103">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="2b1e6-103">Update group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b1e6-104">[グループ](../resources/group.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-104">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b1e6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b1e6-105">Permissions</span></span>

<span data-ttu-id="2b1e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b1e6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b1e6-108">Permission type</span></span>      | <span data-ttu-id="2b1e6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b1e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b1e6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b1e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b1e6-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b1e6-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="2b1e6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b1e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b1e6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-113">Not supported.</span></span>    |
|<span data-ttu-id="2b1e6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b1e6-114">Application</span></span> | <span data-ttu-id="2b1e6-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b1e6-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b1e6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b1e6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b1e6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b1e6-117">Request headers</span></span>

| <span data-ttu-id="2b1e6-118">名前</span><span class="sxs-lookup"><span data-stu-id="2b1e6-118">Name</span></span>       | <span data-ttu-id="2b1e6-119">型</span><span class="sxs-lookup"><span data-stu-id="2b1e6-119">Type</span></span> | <span data-ttu-id="2b1e6-120">説明</span><span class="sxs-lookup"><span data-stu-id="2b1e6-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b1e6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b1e6-121">Authorization</span></span>  | <span data-ttu-id="2b1e6-122">string</span><span class="sxs-lookup"><span data-stu-id="2b1e6-122">string</span></span>  | <span data-ttu-id="2b1e6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b1e6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b1e6-125">Request body</span></span>

<span data-ttu-id="2b1e6-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2b1e6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b1e6-129">Property</span></span>   | <span data-ttu-id="2b1e6-130">型</span><span class="sxs-lookup"><span data-stu-id="2b1e6-130">Type</span></span> |<span data-ttu-id="2b1e6-131">説明</span><span class="sxs-lookup"><span data-stu-id="2b1e6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b1e6-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="2b1e6-132">allowExternalSenders</span></span>|<span data-ttu-id="2b1e6-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b1e6-133">Boolean</span></span>|<span data-ttu-id="2b1e6-p104">既定値は **false** です。組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="2b1e6-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="2b1e6-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="2b1e6-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b1e6-137">Boolean</span></span>|<span data-ttu-id="2b1e6-p105">既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="2b1e6-140">description</span><span class="sxs-lookup"><span data-stu-id="2b1e6-140">description</span></span>|<span data-ttu-id="2b1e6-141">String</span><span class="sxs-lookup"><span data-stu-id="2b1e6-141">String</span></span>|<span data-ttu-id="2b1e6-142">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-142">An optional description for the group.</span></span> |
|<span data-ttu-id="2b1e6-143">displayName</span><span class="sxs-lookup"><span data-stu-id="2b1e6-143">displayName</span></span>|<span data-ttu-id="2b1e6-144">String</span><span class="sxs-lookup"><span data-stu-id="2b1e6-144">String</span></span>|<span data-ttu-id="2b1e6-145">グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-145">The display name for the group.</span></span> <span data-ttu-id="2b1e6-146">このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-146">This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="2b1e6-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="2b1e6-147">groupTypes</span></span>|<span data-ttu-id="2b1e6-148">String collection</span><span class="sxs-lookup"><span data-stu-id="2b1e6-148">String collection</span></span>|<span data-ttu-id="2b1e6-149">グループの種類とそのメンバーシップを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="2b1e6-150">コレクションが**統合**されている場合、グループは Office 365 グループです。それ以外の場合は、セキュリティグループです。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="2b1e6-151">コレクションに**Dynamicmembership**が含まれている場合、そのグループには動的メンバーシップがあります。それ以外の場合、メンバーシップは静的です。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="2b1e6-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="2b1e6-152">mailEnabled</span></span>|<span data-ttu-id="2b1e6-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b1e6-153">Boolean</span></span>|<span data-ttu-id="2b1e6-154">メールが有効なグループであるかどうかを指定します。securityEnabled プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-154">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="2b1e6-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2b1e6-155">mailNickname</span></span>|<span data-ttu-id="2b1e6-156">String</span><span class="sxs-lookup"><span data-stu-id="2b1e6-156">String</span></span>|<span data-ttu-id="2b1e6-157">グループの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-157">The mail alias for the group.</span></span> <span data-ttu-id="2b1e6-158">このプロパティは、グループの作成時に指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="2b1e6-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="2b1e6-159">securityEnabled</span></span>|<span data-ttu-id="2b1e6-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b1e6-160">Boolean</span></span>|<span data-ttu-id="2b1e6-161">グループが Office 365 グループを含むセキュリティグループであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-161">Specifies whether the group is a security group, including Office 365 groups.</span></span> |
|<span data-ttu-id="2b1e6-162">visibility</span><span class="sxs-lookup"><span data-stu-id="2b1e6-162">visibility</span></span>|<span data-ttu-id="2b1e6-163">String</span><span class="sxs-lookup"><span data-stu-id="2b1e6-163">String</span></span>|<span data-ttu-id="2b1e6-p108">Office 365 グループの表示を指定します。使用可能な値は次のとおりです。**Private**、**Public**、または空 (**Public** として解釈されます)。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p108">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="2b1e6-166">**グループ**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、操作を使用して、既存の**グループ**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-166">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="2b1e6-167">**注意:** </span><span class="sxs-lookup"><span data-stu-id="2b1e6-167">**Note:**</span></span>
>
> - <span data-ttu-id="2b1e6-168">**autoSubscribeNewMembers** は、独自の PATCH 要求で指定することによって更新できます。上の表にある他のプロパティは含めません。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-168">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="2b1e6-p109">コア グループの管理とマネージメントに関するグループ API のサブセットのみが、アプリケーションのアクセス許可と委任されたアクセス許可をサポートします。**autoSubscribeNewMembers** の更新を含む他のすべてのグループ API のメンバーは、委任されたアクセス許可のみをサポートします。例については、「[既知の問題](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="2b1e6-172">Microsoft Exchange Server でメールが有効なセキュリティグループを更新するためのルールは複雑になることがあります。詳細については、「 [Exchange Server でメールが有効なセキュリティグループを管理](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-172">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>
 


## <a name="response"></a><span data-ttu-id="2b1e6-173">応答</span><span class="sxs-lookup"><span data-stu-id="2b1e6-173">Response</span></span>

<span data-ttu-id="2b1e6-174">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-174">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2b1e6-175">例</span><span class="sxs-lookup"><span data-stu-id="2b1e6-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2b1e6-176">要求</span><span class="sxs-lookup"><span data-stu-id="2b1e6-176">Request</span></span>

<span data-ttu-id="2b1e6-177">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-177">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2b1e6-178">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2b1e6-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b1e6-179">C#</span><span class="sxs-lookup"><span data-stu-id="2b1e6-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b1e6-180">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b1e6-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b1e6-181">目的-C</span><span class="sxs-lookup"><span data-stu-id="2b1e6-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2b1e6-182">応答</span><span class="sxs-lookup"><span data-stu-id="2b1e6-182">Response</span></span>

<span data-ttu-id="2b1e6-183">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b1e6-183">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="2b1e6-184">関連項目</span><span class="sxs-lookup"><span data-stu-id="2b1e6-184">See also</span></span>

- [<span data-ttu-id="2b1e6-185">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="2b1e6-185">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2b1e6-186">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="2b1e6-186">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2b1e6-187">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="2b1e6-187">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
