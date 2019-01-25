---
title: passwordProfile リソースの種類
description: ユーザーに関連付けられているパスワードのプロファイルが含まれています。**ユーザー** エンティティの **PasswordProfile** プロパティは、passwordProfile オブジェクトです。
localization_priority: Normal
ms.openlocfilehash: 3caff59c8fd0838b91f9fdfb79bdbb154aa83b9f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518934"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="44303-104">passwordProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44303-104">passwordProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44303-p102">ユーザーに関連付けられているパスワードのプロファイルが含まれています。[ユーザー](user.md) エンティティの **PasswordProfile** プロパティは、**passwordProfile** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="44303-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="44303-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44303-107">Properties</span></span>
| <span data-ttu-id="44303-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44303-108">Property</span></span>     | <span data-ttu-id="44303-109">型</span><span class="sxs-lookup"><span data-stu-id="44303-109">Type</span></span>   |<span data-ttu-id="44303-110">説明</span><span class="sxs-lookup"><span data-stu-id="44303-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44303-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="44303-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="44303-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="44303-112">Boolean</span></span>| <span data-ttu-id="44303-113">場合は**true の場合**、次回ログイン時、ユーザーにパスワードを変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44303-113">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="44303-114">パスワードの変更では、このプロパティに自動的がリセットされるまでに \***false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="44303-114">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="44303-115">表示しない場合は、セットでは、既定値は**false**。</span><span class="sxs-lookup"><span data-stu-id="44303-115">If not set, default is **false**.</span></span> |
|<span data-ttu-id="44303-116">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="44303-116">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="44303-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="44303-117">Boolean</span></span>| <span data-ttu-id="44303-118">**True の場合**、次回ログイン時、ユーザーを実行する必要がありますされる前に多要素認証 (MFA) は、パスワードを変更するのには強制します。</span><span class="sxs-lookup"><span data-stu-id="44303-118">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="44303-119">動作は**forceChangePasswordNextSignIn**と同じですが、ユーザーがパスワードを変更する前に最初の多要素認証を実行するために必要な。</span><span class="sxs-lookup"><span data-stu-id="44303-119">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="44303-120">パスワードの変更後このプロパティは自動的にリセットを**false**にします。</span><span class="sxs-lookup"><span data-stu-id="44303-120">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="44303-121">表示しない場合は、セットでは、既定値は**false**。</span><span class="sxs-lookup"><span data-stu-id="44303-121">If not set, default is **false**.</span></span> |
|<span data-ttu-id="44303-122">password</span><span class="sxs-lookup"><span data-stu-id="44303-122">password</span></span>|<span data-ttu-id="44303-123">String</span><span class="sxs-lookup"><span data-stu-id="44303-123">String</span></span>|<span data-ttu-id="44303-p105">ユーザーのパスワード。このプロパティは、ユーザーの作成時に必要です。このプロパティは更新できますが、ユーザーは次回のログインでパスワードを変更する必要があります。パスワードは、ユーザーの **passwordPolicies** プロパティによって指定されているとおりの最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="44303-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44303-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44303-129">JSON representation</span></span>

<span data-ttu-id="44303-130">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="44303-130">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
