---
title: passwordProfile リソースの種類
description: ユーザーに関連付けられているパスワードのプロファイルが含まれています。ユーザー エンティティの **PasswordProfile** プロパティは、**passwordProfile** オブジェクトです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ea3f3daa4807fd56e39930a059d69221e141879c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966235"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="83ecc-104">passwordProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83ecc-104">passwordProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83ecc-p102">ユーザーに関連付けられているパスワードのプロファイルが含まれています。[ユーザー](user.md) エンティティの **PasswordProfile** プロパティは、**passwordProfile** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="83ecc-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="83ecc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83ecc-107">Properties</span></span>
| <span data-ttu-id="83ecc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83ecc-108">Property</span></span>     | <span data-ttu-id="83ecc-109">型</span><span class="sxs-lookup"><span data-stu-id="83ecc-109">Type</span></span>   |<span data-ttu-id="83ecc-110">説明</span><span class="sxs-lookup"><span data-stu-id="83ecc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83ecc-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="83ecc-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="83ecc-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ecc-112">Boolean</span></span>| <span data-ttu-id="83ecc-113">**True**の場合、次のサインイン時に、ユーザーはパスワードを変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83ecc-113">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="83ecc-114">パスワードを変更すると、このプロパティは自動的に \***false**にリセットされます。</span><span class="sxs-lookup"><span data-stu-id="83ecc-114">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="83ecc-115">設定しない場合、既定値は **false** です。</span><span class="sxs-lookup"><span data-stu-id="83ecc-115">If not set, default is **false**.</span></span> |
|<span data-ttu-id="83ecc-116">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="83ecc-116">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="83ecc-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ecc-117">Boolean</span></span>| <span data-ttu-id="83ecc-118">**true** の場合、次回のサインイン時にユーザーは、パスワードの変更を強制される前に多要素認証 (MFA) を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83ecc-118">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="83ecc-119">この動作は **forceChangePasswordNextSignIn** と同じですが、パスワードを変更する前にユーザーが多要素認証を実行する必要がある点が異なります。</span><span class="sxs-lookup"><span data-stu-id="83ecc-119">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="83ecc-120">パスワードを変更すると、このプロパティは自動的に **false** にリセットされます。</span><span class="sxs-lookup"><span data-stu-id="83ecc-120">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="83ecc-121">設定しない場合、既定値は **false** です。</span><span class="sxs-lookup"><span data-stu-id="83ecc-121">If not set, default is **false**.</span></span> |
|<span data-ttu-id="83ecc-122">パスワード</span><span class="sxs-lookup"><span data-stu-id="83ecc-122">password</span></span>|<span data-ttu-id="83ecc-123">String</span><span class="sxs-lookup"><span data-stu-id="83ecc-123">String</span></span>|<span data-ttu-id="83ecc-p105">ユーザーのパスワード。このプロパティは、ユーザーの作成時に必要です。このプロパティは更新できますが、ユーザーは次回のログインでパスワードを変更する必要があります。パスワードは、ユーザーの **passwordPolicies** プロパティによって指定されているとおりの最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="83ecc-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83ecc-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83ecc-129">JSON representation</span></span>

<span data-ttu-id="83ecc-130">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="83ecc-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
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
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
