---
title: グループを更新する
description: グループ オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 53dfecdb34e83288a9bb3f92020750f473ce396a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592422"
---
# <a name="update-group"></a><span data-ttu-id="473f4-103">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="473f4-103">Update group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="473f4-104">[グループ](../resources/group.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="473f4-104">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="473f4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="473f4-105">Permissions</span></span>

<span data-ttu-id="473f4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="473f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="473f4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="473f4-108">Permission type</span></span>      | <span data-ttu-id="473f4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="473f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="473f4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="473f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="473f4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473f4-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="473f4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="473f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="473f4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="473f4-113">Not supported.</span></span>    |
|<span data-ttu-id="473f4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="473f4-114">Application</span></span> | <span data-ttu-id="473f4-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473f4-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="473f4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="473f4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="473f4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="473f4-117">Request headers</span></span>

| <span data-ttu-id="473f4-118">名前</span><span class="sxs-lookup"><span data-stu-id="473f4-118">Name</span></span>       | <span data-ttu-id="473f4-119">型</span><span class="sxs-lookup"><span data-stu-id="473f4-119">Type</span></span> | <span data-ttu-id="473f4-120">説明</span><span class="sxs-lookup"><span data-stu-id="473f4-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="473f4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="473f4-121">Authorization</span></span>  | <span data-ttu-id="473f4-122">string</span><span class="sxs-lookup"><span data-stu-id="473f4-122">string</span></span>  | <span data-ttu-id="473f4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="473f4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="473f4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="473f4-125">Request body</span></span>

<span data-ttu-id="473f4-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="473f4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="473f4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="473f4-129">Property</span></span>   | <span data-ttu-id="473f4-130">型</span><span class="sxs-lookup"><span data-stu-id="473f4-130">Type</span></span> |<span data-ttu-id="473f4-131">説明</span><span class="sxs-lookup"><span data-stu-id="473f4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="473f4-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="473f4-132">allowExternalSenders</span></span>|<span data-ttu-id="473f4-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="473f4-133">Boolean</span></span>|<span data-ttu-id="473f4-p104">既定値は **false** です。組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="473f4-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="473f4-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="473f4-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="473f4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="473f4-137">Boolean</span></span>|<span data-ttu-id="473f4-p105">既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="473f4-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="473f4-140">description</span><span class="sxs-lookup"><span data-stu-id="473f4-140">description</span></span>|<span data-ttu-id="473f4-141">String</span><span class="sxs-lookup"><span data-stu-id="473f4-141">String</span></span>|<span data-ttu-id="473f4-142">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="473f4-142">An optional description for the group.</span></span> |
|<span data-ttu-id="473f4-143">displayName</span><span class="sxs-lookup"><span data-stu-id="473f4-143">displayName</span></span>|<span data-ttu-id="473f4-144">String</span><span class="sxs-lookup"><span data-stu-id="473f4-144">String</span></span>|<span data-ttu-id="473f4-p106">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="473f4-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="473f4-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="473f4-148">groupTypes</span></span>|<span data-ttu-id="473f4-149">String collection</span><span class="sxs-lookup"><span data-stu-id="473f4-149">String collection</span></span>|<span data-ttu-id="473f4-p107">作成するグループの種類を指定します。使用可能な値は **Unified** (Office 365 のグループを作成する場合) または **DynamicMembership** (動的なグループを作成する場合) です。その他のグループの種類 (セキュリティが有効なグループやメールが有効なセキュリティ グループなど) の場合、このプロパティは設定しないでください。</span><span class="sxs-lookup"><span data-stu-id="473f4-p107">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="473f4-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="473f4-153">mailEnabled</span></span>|<span data-ttu-id="473f4-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="473f4-154">Boolean</span></span>|<span data-ttu-id="473f4-p108">メールが有効なグループであるかどうかを指定します。**securityEnabled** プロパティも **true** の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、Microsoft Exchange 配布グループになります。</span><span class="sxs-lookup"><span data-stu-id="473f4-p108">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="473f4-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="473f4-157">mailNickname</span></span>|<span data-ttu-id="473f4-158">String</span><span class="sxs-lookup"><span data-stu-id="473f4-158">String</span></span>|<span data-ttu-id="473f4-p109">グループの電子メール エイリアス。このプロパティは、グループの作成時に指定する必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="473f4-p109">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="473f4-162">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="473f4-162">securityEnabled</span></span>|<span data-ttu-id="473f4-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="473f4-163">Boolean</span></span>|<span data-ttu-id="473f4-p110">グループがセキュリティ グループであるかどうかを指定します。**mailEnabled** プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、セキュリティ グループになります。Office 365 グループの場合、**false** にする必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="473f4-p110">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="473f4-168">visibility</span><span class="sxs-lookup"><span data-stu-id="473f4-168">visibility</span></span>|<span data-ttu-id="473f4-169">String</span><span class="sxs-lookup"><span data-stu-id="473f4-169">String</span></span>|<span data-ttu-id="473f4-p111">Office 365 グループの表示を指定します。使用可能な値は次のとおりです。**Private**、**Public**、または空 (**Public** として解釈されます)。</span><span class="sxs-lookup"><span data-stu-id="473f4-p111">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="473f4-172">**グループ**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、操作を使用して、既存の**グループ**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="473f4-172">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>

> <span data-ttu-id="473f4-173">**注意:** </span><span class="sxs-lookup"><span data-stu-id="473f4-173">**Note:**</span></span>
>
> - <span data-ttu-id="473f4-174">**autoSubscribeNewMembers** は、独自の PATCH 要求で指定することによって更新できます。上の表にある他のプロパティは含めません。</span><span class="sxs-lookup"><span data-stu-id="473f4-174">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="473f4-p112">コア グループの管理とマネージメントに関するグループ API のサブセットのみが、アプリケーションのアクセス許可と委任されたアクセス許可をサポートします。**autoSubscribeNewMembers** の更新を含む他のすべてのグループ API のメンバーは、委任されたアクセス許可のみをサポートします。例については、「[既知の問題](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="473f4-p112">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="473f4-178">応答</span><span class="sxs-lookup"><span data-stu-id="473f4-178">Response</span></span>

<span data-ttu-id="473f4-179">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="473f4-179">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="473f4-180">例</span><span class="sxs-lookup"><span data-stu-id="473f4-180">Example</span></span>

#### <a name="request"></a><span data-ttu-id="473f4-181">要求</span><span class="sxs-lookup"><span data-stu-id="473f4-181">Request</span></span>

<span data-ttu-id="473f4-182">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="473f4-182">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="473f4-183">応答</span><span class="sxs-lookup"><span data-stu-id="473f4-183">Response</span></span>

<span data-ttu-id="473f4-184">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="473f4-184">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="473f4-185">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="473f4-185">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="473f4-186">Visual</span><span class="sxs-lookup"><span data-stu-id="473f4-186">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="473f4-187">Java</span><span class="sxs-lookup"><span data-stu-id="473f4-187">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="473f4-188">関連項目</span><span class="sxs-lookup"><span data-stu-id="473f4-188">See also</span></span>

- [<span data-ttu-id="473f4-189">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="473f4-189">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="473f4-190">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="473f4-190">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="473f4-191">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="473f4-191">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/group-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
