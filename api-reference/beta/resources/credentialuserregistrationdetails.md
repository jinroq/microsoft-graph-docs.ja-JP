---
title: credentialUserRegistrationDetails リソースの種類
description: 登録されているすべてのユーザーに対して、セルフサービスのパスワードのリセットと多要素認証 (MFA) の使用法の詳細を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 414cd6977f4e3c15ab7b82bd88329e9e3549f137
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527085"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="3f3b3-103">credentialUserRegistrationDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3f3b3-103">credentialUserRegistrationDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f3b3-104">登録されているすべてのユーザーに対して、セルフサービスのパスワードのリセットと多要素認証 (MFA) の使用法の詳細を表します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-104">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="3f3b3-105">詳細には、ユーザー情報、登録の状態、使用される認証方法が含まれます。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-105">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="3f3b3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f3b3-106">Methods</span></span>

| <span data-ttu-id="3f3b3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f3b3-107">Method</span></span>       | <span data-ttu-id="3f3b3-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3f3b3-108">Return Type</span></span> | <span data-ttu-id="3f3b3-109">説明</span><span class="sxs-lookup"><span data-stu-id="3f3b3-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3f3b3-110">CredentialUserRegistrationDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3f3b3-110">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="3f3b3-111">credentialUserRegistrationDetails コレクション</span><span class="sxs-lookup"><span data-stu-id="3f3b3-111">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="3f3b3-112">指定したテナントの[Credentialuserregistrationdetails](../resources/credentialuserregistrationdetails.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-112">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="3f3b3-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f3b3-113">Properties</span></span>

| <span data-ttu-id="3f3b3-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f3b3-114">Property</span></span>     | <span data-ttu-id="3f3b3-115">型</span><span class="sxs-lookup"><span data-stu-id="3f3b3-115">Type</span></span>        | <span data-ttu-id="3f3b3-116">説明</span><span class="sxs-lookup"><span data-stu-id="3f3b3-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3f3b3-117">authMethods</span><span class="sxs-lookup"><span data-stu-id="3f3b3-117">authMethods</span></span> | <span data-ttu-id="3f3b3-118">registrationAuthMethod コレクション</span><span class="sxs-lookup"><span data-stu-id="3f3b3-118">registrationAuthMethod collection</span></span> | <span data-ttu-id="3f3b3-119">ユーザーが使用した認証方法を表します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="3f3b3-120">可能な値は`email`、 `mobilePhone` `officePhone`、、 `securityQuestion` 、(セルフサービスのパスワードのリセットにのみ使用`appNotification`) `appCode`、、 `alternateMobilePhone` 、および (登録でのみサポートされます) です。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-120">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="3f3b3-121">id</span><span class="sxs-lookup"><span data-stu-id="3f3b3-121">id</span></span> | <span data-ttu-id="3f3b3-122">文字列</span><span class="sxs-lookup"><span data-stu-id="3f3b3-122">String</span></span> | <span data-ttu-id="3f3b3-123">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-123">The unique identifier for the activity.</span></span> <span data-ttu-id="3f3b3-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-124">Read-only.</span></span>|
| <span data-ttu-id="3f3b3-125">isCapable</span><span class="sxs-lookup"><span data-stu-id="3f3b3-125">isCapable</span></span> | <span data-ttu-id="3f3b3-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f3b3-126">Boolean</span></span> | <span data-ttu-id="3f3b3-127">ユーザーがセルフサービスのパスワードのリセットまたは MFA を実行する準備ができているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-127">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="3f3b3-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3f3b3-128">isEnabled</span></span> | <span data-ttu-id="3f3b3-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f3b3-129">Boolean</span></span> | <span data-ttu-id="3f3b3-130">ユーザーがセルフサービスのパスワードのリセットの実行を有効にしたかどうかを Indiciates します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-130">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="3f3b3-131">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="3f3b3-131">isMfaRegistered</span></span> | <span data-ttu-id="3f3b3-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f3b3-132">Boolean</span></span> | <span data-ttu-id="3f3b3-133">ユーザーが MFA 用に登録されているかどうかを Indiciates します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-133">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="3f3b3-134">isRegistered</span><span class="sxs-lookup"><span data-stu-id="3f3b3-134">isRegistered</span></span> | <span data-ttu-id="3f3b3-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f3b3-135">Boolean</span></span> | <span data-ttu-id="3f3b3-136">ユーザーがセルフサービスのパスワードのリセットのために認証方法を登録しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-136">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="3f3b3-137">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3f3b3-137">userDisplayName</span></span> | <span data-ttu-id="3f3b3-138">String</span><span class="sxs-lookup"><span data-stu-id="3f3b3-138">String</span></span> | <span data-ttu-id="3f3b3-139">対応するユーザーのユーザー名を提供します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-139">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="3f3b3-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3f3b3-140">userPrincipalName</span></span> | <span data-ttu-id="3f3b3-141">String</span><span class="sxs-lookup"><span data-stu-id="3f3b3-141">String</span></span> | <span data-ttu-id="3f3b3-142">対応するユーザーのユーザープリンシパル名を提供します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-142">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3f3b3-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3f3b3-143">Relationships</span></span>

<span data-ttu-id="3f3b3-144">なし。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f3b3-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3f3b3-145">JSON representation</span></span>

<span data-ttu-id="3f3b3-146">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3f3b3-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "authMethods": ["string"],
  "isRegistered" : false,
  "isEnabled" : true,
  "isCapable" : false,
  "isMfaRegistered" : true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->