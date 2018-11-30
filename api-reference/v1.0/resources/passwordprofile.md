---
title: passwordProfile リソースの種類
description: ユーザーに関連付けられているパスワードのプロファイルが含まれています。ユーザー エンティティの **PasswordProfile** プロパティは、**passwordProfile** オブジェクトです。
ms.openlocfilehash: ee933b75b3dc536cbfcb33502cdda0d63680174c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022970"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="91d73-104">passwordProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91d73-104">passwordProfile resource type</span></span>

<span data-ttu-id="91d73-p102">ユーザーに関連付けられているパスワードのプロファイルが含まれています。[ユーザー](user.md) エンティティの **PasswordProfile** プロパティは、**passwordProfile** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="91d73-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="91d73-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91d73-107">Properties</span></span>
| <span data-ttu-id="91d73-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91d73-108">Property</span></span>     | <span data-ttu-id="91d73-109">型</span><span class="sxs-lookup"><span data-stu-id="91d73-109">Type</span></span>   |<span data-ttu-id="91d73-110">説明</span><span class="sxs-lookup"><span data-stu-id="91d73-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91d73-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="91d73-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="91d73-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="91d73-112">Boolean</span></span>| <span data-ttu-id="91d73-113">ユーザーが次回のログインでパスワードを変更する必要がある場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="91d73-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="91d73-114">password</span><span class="sxs-lookup"><span data-stu-id="91d73-114">password</span></span>|<span data-ttu-id="91d73-115">String</span><span class="sxs-lookup"><span data-stu-id="91d73-115">String</span></span>|<span data-ttu-id="91d73-p103">ユーザーのパスワード。このプロパティは、ユーザーの作成時に必要です。このプロパティは更新できますが、ユーザーは次回のログインでパスワードを変更する必要があります。パスワードは、ユーザーの **passwordPolicies** プロパティによって指定されているとおりの最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="91d73-p103">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91d73-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91d73-121">JSON representation</span></span>

<span data-ttu-id="91d73-122">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="91d73-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
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