---
title: グループを更新する
description: グループ オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7974d9db9216a013e01c5f12f87f74488ab929ea
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373372"
---
# <a name="update-group"></a><span data-ttu-id="e0b7a-103">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="e0b7a-103">Update group</span></span>

<span data-ttu-id="e0b7a-104">グループ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-104">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0b7a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e0b7a-105">Permissions</span></span>

<span data-ttu-id="e0b7a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0b7a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0b7a-108">Permission type</span></span>      | <span data-ttu-id="e0b7a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0b7a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0b7a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0b7a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0b7a-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0b7a-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="e0b7a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0b7a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0b7a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-113">Not supported.</span></span>    |
|<span data-ttu-id="e0b7a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0b7a-114">Application</span></span> | <span data-ttu-id="e0b7a-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b7a-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0b7a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0b7a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e0b7a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0b7a-117">Request headers</span></span>

| <span data-ttu-id="e0b7a-118">名前</span><span class="sxs-lookup"><span data-stu-id="e0b7a-118">Name</span></span>       | <span data-ttu-id="e0b7a-119">種類</span><span class="sxs-lookup"><span data-stu-id="e0b7a-119">Type</span></span> | <span data-ttu-id="e0b7a-120">説明</span><span class="sxs-lookup"><span data-stu-id="e0b7a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0b7a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0b7a-121">Authorization</span></span>  | <span data-ttu-id="e0b7a-122">string</span><span class="sxs-lookup"><span data-stu-id="e0b7a-122">string</span></span>  | <span data-ttu-id="e0b7a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0b7a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0b7a-125">Request body</span></span>

<span data-ttu-id="e0b7a-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e0b7a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0b7a-129">Property</span></span>   | <span data-ttu-id="e0b7a-130">型</span><span class="sxs-lookup"><span data-stu-id="e0b7a-130">Type</span></span> |<span data-ttu-id="e0b7a-131">説明</span><span class="sxs-lookup"><span data-stu-id="e0b7a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0b7a-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="e0b7a-132">allowExternalSenders</span></span>|<span data-ttu-id="e0b7a-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0b7a-133">Boolean</span></span>|<span data-ttu-id="e0b7a-p104">既定値は **false** です。組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="e0b7a-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="e0b7a-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="e0b7a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0b7a-137">Boolean</span></span>|<span data-ttu-id="e0b7a-p105">既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="e0b7a-140">description</span><span class="sxs-lookup"><span data-stu-id="e0b7a-140">description</span></span>|<span data-ttu-id="e0b7a-141">String</span><span class="sxs-lookup"><span data-stu-id="e0b7a-141">String</span></span>|<span data-ttu-id="e0b7a-142">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-142">An optional description for the group.</span></span> |
|<span data-ttu-id="e0b7a-143">displayName</span><span class="sxs-lookup"><span data-stu-id="e0b7a-143">displayName</span></span>|<span data-ttu-id="e0b7a-144">String</span><span class="sxs-lookup"><span data-stu-id="e0b7a-144">String</span></span>|<span data-ttu-id="e0b7a-p106">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span> |
|<span data-ttu-id="e0b7a-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="e0b7a-147">groupTypes</span></span>|<span data-ttu-id="e0b7a-148">String collection</span><span class="sxs-lookup"><span data-stu-id="e0b7a-148">String collection</span></span>|<span data-ttu-id="e0b7a-149">グループの種類とそのメンバーシップを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="e0b7a-150">コレクションに **Unified** が含まれている場合、そのグループは Office 365 グループです。それ以外の場合はセキュリティ グループです。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="e0b7a-151">コレクションに **DynamicMembership** が含まれている場合、そのグループには動的メンバーシップがあります。それ以外の場合は、メンバーシップは静的です。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="e0b7a-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="e0b7a-152">mailEnabled</span></span>|<span data-ttu-id="e0b7a-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="e0b7a-153">Boolean</span></span>|<span data-ttu-id="e0b7a-154">メールが有効なグループであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-154">Specifies whether the group is mail-enabled.</span></span>|
|<span data-ttu-id="e0b7a-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e0b7a-155">mailNickname</span></span>|<span data-ttu-id="e0b7a-156">文字列</span><span class="sxs-lookup"><span data-stu-id="e0b7a-156">String</span></span>|<span data-ttu-id="e0b7a-157">グループの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-157">The mail alias for the group.</span></span> <span data-ttu-id="e0b7a-158">このプロパティは、グループの作成時に指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="e0b7a-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="e0b7a-159">securityEnabled</span></span>|<span data-ttu-id="e0b7a-160">ブール値</span><span class="sxs-lookup"><span data-stu-id="e0b7a-160">Boolean</span></span>|<span data-ttu-id="e0b7a-161">グループがセキュリティ グループであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-161">Specifies whether the group is a security group.</span></span> |
|<span data-ttu-id="e0b7a-162">visibility</span><span class="sxs-lookup"><span data-stu-id="e0b7a-162">visibility</span></span>|<span data-ttu-id="e0b7a-163">String</span><span class="sxs-lookup"><span data-stu-id="e0b7a-163">String</span></span>|<span data-ttu-id="e0b7a-164">Office 365 グループの表示を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-164">Specifies the visibility of an Office 365 group.</span></span> <span data-ttu-id="e0b7a-165">可能な値は以下のどれかです: **Private**、**Public**または empty (これは **Public**と解釈されます)。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-165">The possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

> <span data-ttu-id="e0b7a-166">**注意:** </span><span class="sxs-lookup"><span data-stu-id="e0b7a-166">**Note:**</span></span>
>
> - <span data-ttu-id="e0b7a-167">上記の表に他のプロパティを含めずに、独自のPATCHリクエストで指定して**autoSubscribeNewMembers**を更新することができます。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-167">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request,without including the other properties in the table above.</span></span>
> - <span data-ttu-id="e0b7a-p109">コア グループの管理とマネージメントに関するグループ API のサブセットのみが、アプリケーションのアクセス許可と委任されたアクセス許可をサポートします。**autoSubscribeNewMembers** の更新を含む他のすべてのグループ API のメンバーは、委任されたアクセス許可のみをサポートします。例については、「[既知の問題](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="e0b7a-171">Microsoft Exchange Server でメールが有効なセキュリティ グループを更新するためのルールが複雑になる場合があります。詳細については、「[Exchange Server でメールが有効なセキュリティ グループを管理する](https://docs.microsoft.com/ja-JP/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-171">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>


## <a name="response"></a><span data-ttu-id="e0b7a-172">応答</span><span class="sxs-lookup"><span data-stu-id="e0b7a-172">Response</span></span>

<span data-ttu-id="e0b7a-173">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-173">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e0b7a-174">例</span><span class="sxs-lookup"><span data-stu-id="e0b7a-174">Example</span></span>

<span data-ttu-id="e0b7a-175">次の例は、グループを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-175">The following example shows how to create a management scope for a specific group.</span></span>

### <a name="request"></a><span data-ttu-id="e0b7a-176">要求</span><span class="sxs-lookup"><span data-stu-id="e0b7a-176">Request</span></span>

<span data-ttu-id="e0b7a-177">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-177">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e0b7a-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0b7a-178">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0b7a-179">C#</span><span class="sxs-lookup"><span data-stu-id="e0b7a-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0b7a-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0b7a-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0b7a-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0b7a-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e0b7a-182">Java</span><span class="sxs-lookup"><span data-stu-id="e0b7a-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e0b7a-183">応答</span><span class="sxs-lookup"><span data-stu-id="e0b7a-183">Response</span></span>

<span data-ttu-id="e0b7a-184">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e0b7a-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
