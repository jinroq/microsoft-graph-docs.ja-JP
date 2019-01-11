---
title: passwordProfile リソースの種類
description: ユーザーに関連付けられているパスワードのプロファイルが含まれています。ユーザー エンティティの **PasswordProfile** プロパティは、**passwordProfile** オブジェクトです。
localization_priority: Normal
ms.openlocfilehash: 11930b046fafaf89f8db751891b9b7f2f72fd99d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839005"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="95359-104">passwordProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95359-104">passwordProfile resource type</span></span>

> <span data-ttu-id="95359-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95359-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95359-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95359-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95359-p103">ユーザーに関連付けられているパスワードのプロファイルが含まれています。[ユーザー](user.md) エンティティの **PasswordProfile** プロパティは、**passwordProfile** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="95359-p103">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="95359-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95359-109">Properties</span></span>
| <span data-ttu-id="95359-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95359-110">Property</span></span>     | <span data-ttu-id="95359-111">種類</span><span class="sxs-lookup"><span data-stu-id="95359-111">Type</span></span>   |<span data-ttu-id="95359-112">説明</span><span class="sxs-lookup"><span data-stu-id="95359-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95359-113">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="95359-113">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="95359-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="95359-114">Boolean</span></span>| <span data-ttu-id="95359-115">場合は**true の場合**、次回ログイン時、ユーザーにパスワードを変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="95359-115">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="95359-116">パスワードの変更では、このプロパティに自動的がリセットされるまでに \***false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="95359-116">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="95359-117">表示しない場合は、セットでは、既定値は**false**。</span><span class="sxs-lookup"><span data-stu-id="95359-117">If not set, default is **false**.</span></span> |
|<span data-ttu-id="95359-118">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="95359-118">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="95359-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="95359-119">Boolean</span></span>| <span data-ttu-id="95359-120">**True の場合**、次回ログイン時、ユーザーを実行する必要がありますされる前に多要素認証 (MFA) は、パスワードを変更するのには強制します。</span><span class="sxs-lookup"><span data-stu-id="95359-120">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="95359-121">動作は**forceChangePasswordNextSignIn**と同じですが、ユーザーがパスワードを変更する前に最初の多要素認証を実行するために必要な。</span><span class="sxs-lookup"><span data-stu-id="95359-121">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="95359-122">パスワードの変更後このプロパティは自動的にリセットを**false**にします。</span><span class="sxs-lookup"><span data-stu-id="95359-122">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="95359-123">表示しない場合は、セットでは、既定値は**false**。</span><span class="sxs-lookup"><span data-stu-id="95359-123">If not set, default is **false**.</span></span> |
|<span data-ttu-id="95359-124">password</span><span class="sxs-lookup"><span data-stu-id="95359-124">password</span></span>|<span data-ttu-id="95359-125">String</span><span class="sxs-lookup"><span data-stu-id="95359-125">String</span></span>|<span data-ttu-id="95359-p106">ユーザーのパスワード。このプロパティは、ユーザーの作成時に必要です。このプロパティは更新できますが、ユーザーは次回のログインでパスワードを変更する必要があります。パスワードは、ユーザーの **passwordPolicies** プロパティによって指定されているとおりの最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="95359-p106">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95359-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95359-131">JSON representation</span></span>

<span data-ttu-id="95359-132">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="95359-132">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": false,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
