---
title: credentialUsageSummary リソースの種類
description: 組織内のユーザーのうち、セルフサービスのパスワードのリセット機能を使用しているユーザー数の現在の状態を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 46fc3f90b7a7f286d61a324e7b5f439d467a4978
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527086"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="d5ee5-103">credentialUsageSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5ee5-103">credentialUsageSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5ee5-104">組織内のユーザーのうち、セルフサービスのパスワードのリセット機能を使用しているユーザー数の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-104">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="d5ee5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d5ee5-105">Methods</span></span>

| <span data-ttu-id="d5ee5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d5ee5-106">Method</span></span>       | <span data-ttu-id="d5ee5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d5ee5-107">Return Type</span></span> | <span data-ttu-id="d5ee5-108">説明</span><span class="sxs-lookup"><span data-stu-id="d5ee5-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d5ee5-109">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="d5ee5-109">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="d5ee5-110">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="d5ee5-110">credentialUsageSummary</span></span> | <span data-ttu-id="d5ee5-111">CredentialUsageSummary オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-111">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d5ee5-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5ee5-112">Properties</span></span>

| <span data-ttu-id="d5ee5-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5ee5-113">Property</span></span>     | <span data-ttu-id="d5ee5-114">型</span><span class="sxs-lookup"><span data-stu-id="d5ee5-114">Type</span></span>        | <span data-ttu-id="d5ee5-115">説明</span><span class="sxs-lookup"><span data-stu-id="d5ee5-115">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d5ee5-116">authMethod</span><span class="sxs-lookup"><span data-stu-id="d5ee5-116">authMethod</span></span> | <span data-ttu-id="d5ee5-117">string</span><span class="sxs-lookup"><span data-stu-id="d5ee5-117">string</span></span> | <span data-ttu-id="d5ee5-118">ユーザーが使用した認証方法を表します。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-118">Represents the authentication method that the user used.</span></span> <span data-ttu-id="d5ee5-119">可能な値は`email`、 `mobileSMS` `mobileCall`、、 `officePhone`、 `securityQuestion` 、(セルフサービスのパスワードのリセットにのみ使用`appNotification`さ`appCode`れます`alternateMobileCall` )、、、および (登録に対してのみサポートされています)。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-119">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="d5ee5-120">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="d5ee5-120">failureActivityCount</span></span> | <span data-ttu-id="d5ee5-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ee5-121">Int64</span></span> | <span data-ttu-id="d5ee5-122">失敗したリセットまたは登録データのカウントを提供します。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-122">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="d5ee5-123">特徴</span><span class="sxs-lookup"><span data-stu-id="d5ee5-123">feature</span></span> | <span data-ttu-id="d5ee5-124">string</span><span class="sxs-lookup"><span data-stu-id="d5ee5-124">string</span></span> | <span data-ttu-id="d5ee5-125">レポートする機能を定義します。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-125">Defines the feature to report.</span></span> <span data-ttu-id="d5ee5-126">可能な値は`registration` 、 `reset`とです。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-126">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="d5ee5-127">id</span><span class="sxs-lookup"><span data-stu-id="d5ee5-127">id</span></span> | <span data-ttu-id="d5ee5-128">String</span><span class="sxs-lookup"><span data-stu-id="d5ee5-128">String</span></span> | <span data-ttu-id="d5ee5-129">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-129">The unique identifier for the activity.</span></span> <span data-ttu-id="d5ee5-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-130">Read-only.</span></span> |
| <span data-ttu-id="d5ee5-131">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="d5ee5-131">successfulActivityCount</span></span> | <span data-ttu-id="d5ee5-132">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ee5-132">Int64</span></span> | <span data-ttu-id="d5ee5-133">成功した登録またはリセットの数を提供します。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-133">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d5ee5-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d5ee5-134">Relationships</span></span>

<span data-ttu-id="d5ee5-135">なし。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5ee5-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5ee5-136">JSON representation</span></span>

<span data-ttu-id="d5ee5-137">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d5ee5-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "successfulActivityCount":"Int64",
  "failureActivityCount": "Int64",
  "authMethod": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUsageSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->