---
title: credentialUserRegistrationCount リソースの種類
description: 組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証機能を使用するために登録されているユーザーの数の現在の状態を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 42c722b04493767d3dbcaf713157d931569d8c32
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485265"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="81b9b-103">credentialUserRegistrationCount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81b9b-103">credentialUserRegistrationCount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81b9b-104">組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証機能を使用するために登録されているユーザーの数の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="81b9b-104">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="81b9b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="81b9b-105">Methods</span></span>

| <span data-ttu-id="81b9b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="81b9b-106">Method</span></span>       | <span data-ttu-id="81b9b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="81b9b-107">Return Type</span></span> | <span data-ttu-id="81b9b-108">説明</span><span class="sxs-lookup"><span data-stu-id="81b9b-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="81b9b-109">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="81b9b-109">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="81b9b-110">credentialUserRegistrationCount コレクション</span><span class="sxs-lookup"><span data-stu-id="81b9b-110">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="81b9b-111">組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証 (MFA) の機能を使用するために登録されているユーザー数の現在の状態を報告します。</span><span class="sxs-lookup"><span data-stu-id="81b9b-111">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="81b9b-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81b9b-112">Properties</span></span>

| <span data-ttu-id="81b9b-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81b9b-113">Property</span></span>     | <span data-ttu-id="81b9b-114">型</span><span class="sxs-lookup"><span data-stu-id="81b9b-114">Type</span></span>        | <span data-ttu-id="81b9b-115">説明</span><span class="sxs-lookup"><span data-stu-id="81b9b-115">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="81b9b-116">id</span><span class="sxs-lookup"><span data-stu-id="81b9b-116">id</span></span> | <span data-ttu-id="81b9b-117">String</span><span class="sxs-lookup"><span data-stu-id="81b9b-117">String</span></span> | <span data-ttu-id="81b9b-118">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="81b9b-118">The unique identifier for the activity.</span></span> <span data-ttu-id="81b9b-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="81b9b-119">Read-only.</span></span> |
| <span data-ttu-id="81b9b-120">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="81b9b-120">totalUserCount</span></span> | <span data-ttu-id="81b9b-121">Int64</span><span class="sxs-lookup"><span data-stu-id="81b9b-121">Int64</span></span> | <span data-ttu-id="81b9b-122">テナント内の総ユーザー数を示します。</span><span class="sxs-lookup"><span data-stu-id="81b9b-122">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="81b9b-123">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="81b9b-123">userRegistrationCounts</span></span> | <span data-ttu-id="81b9b-124">[Userregistrationcount](userregistrationcount.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="81b9b-124">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="81b9b-125">テナント内のユーザーの登録数と状態情報のコレクション。</span><span class="sxs-lookup"><span data-stu-id="81b9b-125">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="81b9b-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81b9b-126">Relationships</span></span>

<span data-ttu-id="81b9b-127">なし。</span><span class="sxs-lookup"><span data-stu-id="81b9b-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81b9b-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81b9b-128">JSON representation</span></span>

<span data-ttu-id="81b9b-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="81b9b-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "totalUserCount" : 23123,
  "userRegistrationCounts" :
  [
    { "registrationStatus":"registered", "registrationCount": 23423 },
    { "registrationStatus":"enabled", "registrationCount": 4234 },
    { "registrationStatus":"capable", "registrationCount": 323 },
    { "registrationStatus":"mfaRegistered", "registrationCount": 33 }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->