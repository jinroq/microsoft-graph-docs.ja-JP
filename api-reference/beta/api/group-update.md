---
title: グループを更新する
description: グループ オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f1f86067771a4732c8839f48bc02dd3edd15c19b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915236"
---
# <a name="update-group"></a><span data-ttu-id="5b9dc-103">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="5b9dc-103">Update group</span></span>

> <span data-ttu-id="5b9dc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b9dc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b9dc-106">[グループ](../resources/group.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-106">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b9dc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b9dc-107">Permissions</span></span>

<span data-ttu-id="5b9dc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b9dc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b9dc-110">Permission type</span></span>      | <span data-ttu-id="5b9dc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b9dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b9dc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b9dc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b9dc-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b9dc-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b9dc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b9dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b9dc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-115">Not supported.</span></span>    |
|<span data-ttu-id="5b9dc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b9dc-116">Application</span></span> | <span data-ttu-id="5b9dc-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b9dc-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b9dc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b9dc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5b9dc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b9dc-119">Request headers</span></span>

| <span data-ttu-id="5b9dc-120">名前</span><span class="sxs-lookup"><span data-stu-id="5b9dc-120">Name</span></span>       | <span data-ttu-id="5b9dc-121">種類</span><span class="sxs-lookup"><span data-stu-id="5b9dc-121">Type</span></span> | <span data-ttu-id="5b9dc-122">説明</span><span class="sxs-lookup"><span data-stu-id="5b9dc-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5b9dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b9dc-123">Authorization</span></span>  | <span data-ttu-id="5b9dc-124">string</span><span class="sxs-lookup"><span data-stu-id="5b9dc-124">string</span></span>  | <span data-ttu-id="5b9dc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b9dc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b9dc-127">Request body</span></span>

<span data-ttu-id="5b9dc-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5b9dc-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b9dc-131">Property</span></span>   | <span data-ttu-id="5b9dc-132">種類</span><span class="sxs-lookup"><span data-stu-id="5b9dc-132">Type</span></span> |<span data-ttu-id="5b9dc-133">説明</span><span class="sxs-lookup"><span data-stu-id="5b9dc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b9dc-134">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="5b9dc-134">allowExternalSenders</span></span>|<span data-ttu-id="5b9dc-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="5b9dc-135">Boolean</span></span>|<span data-ttu-id="5b9dc-p105">既定値は **false** です。組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p105">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="5b9dc-138">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="5b9dc-138">autoSubscribeNewMembers</span></span>|<span data-ttu-id="5b9dc-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="5b9dc-139">Boolean</span></span>|<span data-ttu-id="5b9dc-p106">既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p106">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="5b9dc-142">説明</span><span class="sxs-lookup"><span data-stu-id="5b9dc-142">description</span></span>|<span data-ttu-id="5b9dc-143">String</span><span class="sxs-lookup"><span data-stu-id="5b9dc-143">String</span></span>|<span data-ttu-id="5b9dc-144">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-144">An optional description for the group.</span></span> |
|<span data-ttu-id="5b9dc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5b9dc-145">displayName</span></span>|<span data-ttu-id="5b9dc-146">String</span><span class="sxs-lookup"><span data-stu-id="5b9dc-146">String</span></span>|<span data-ttu-id="5b9dc-p107">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p107">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="5b9dc-150">groupTypes</span><span class="sxs-lookup"><span data-stu-id="5b9dc-150">groupTypes</span></span>|<span data-ttu-id="5b9dc-151">String collection</span><span class="sxs-lookup"><span data-stu-id="5b9dc-151">String collection</span></span>|<span data-ttu-id="5b9dc-p108">作成するグループの種類を指定します。使用可能な値は **Unified** (Office 365 のグループを作成する場合) または **DynamicMembership** (動的なグループを作成する場合) です。その他のグループの種類 (セキュリティが有効なグループやメールが有効なセキュリティ グループなど) の場合、このプロパティは設定しないでください。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p108">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="5b9dc-155">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="5b9dc-155">mailEnabled</span></span>|<span data-ttu-id="5b9dc-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b9dc-156">Boolean</span></span>|<span data-ttu-id="5b9dc-p109">メールが有効なグループであるかどうかを指定します。**securityEnabled** プロパティも **true** の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、Microsoft Exchange 配布グループになります。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p109">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="5b9dc-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5b9dc-159">mailNickname</span></span>|<span data-ttu-id="5b9dc-160">String</span><span class="sxs-lookup"><span data-stu-id="5b9dc-160">String</span></span>|<span data-ttu-id="5b9dc-p110">グループの電子メール エイリアス。このプロパティは、グループの作成時に指定する必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p110">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="5b9dc-164">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="5b9dc-164">securityEnabled</span></span>|<span data-ttu-id="5b9dc-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b9dc-165">Boolean</span></span>|<span data-ttu-id="5b9dc-p111">グループがセキュリティ グループであるかどうかを指定します。**mailEnabled** プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、セキュリティ グループになります。Office 365 グループの場合、**false** にする必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p111">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="5b9dc-170">visibility</span><span class="sxs-lookup"><span data-stu-id="5b9dc-170">visibility</span></span>|<span data-ttu-id="5b9dc-171">String</span><span class="sxs-lookup"><span data-stu-id="5b9dc-171">String</span></span>|<span data-ttu-id="5b9dc-p112">Office 365 グループの表示を指定します。使用可能な値は次のとおりです。**Private**、**Public**、または空 (**Public** として解釈されます)。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p112">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="5b9dc-174">**グループ**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用すること、`PATCH`を追加、更新、または既存の**グループ**のインスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-174">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>

> <span data-ttu-id="5b9dc-175">**注:** </span><span class="sxs-lookup"><span data-stu-id="5b9dc-175">**Note:**</span></span>
>
> - <span data-ttu-id="5b9dc-176">**autoSubscribeNewMembers** は、独自の PATCH 要求で指定することによって更新できます。上の表にある他のプロパティは含めません。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-176">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="5b9dc-p113">コア グループの管理とマネージメントに関するグループ API のサブセットのみが、アプリケーションのアクセス許可と委任されたアクセス許可をサポートします。**autoSubscribeNewMembers** の更新を含む他のすべてのグループ API のメンバーは、委任されたアクセス許可のみをサポートします。例については、「[既知の問題](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-p113">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="5b9dc-180">応答</span><span class="sxs-lookup"><span data-stu-id="5b9dc-180">Response</span></span>

<span data-ttu-id="5b9dc-181">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-181">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5b9dc-182">例</span><span class="sxs-lookup"><span data-stu-id="5b9dc-182">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5b9dc-183">要求</span><span class="sxs-lookup"><span data-stu-id="5b9dc-183">Request</span></span>

<span data-ttu-id="5b9dc-184">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-184">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="5b9dc-185">応答</span><span class="sxs-lookup"><span data-stu-id="5b9dc-185">Response</span></span>

<span data-ttu-id="5b9dc-186">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b9dc-186">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="5b9dc-187">関連項目</span><span class="sxs-lookup"><span data-stu-id="5b9dc-187">See also</span></span>

- [<span data-ttu-id="5b9dc-188">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="5b9dc-188">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5b9dc-189">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="5b9dc-189">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5b9dc-190">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="5b9dc-190">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
