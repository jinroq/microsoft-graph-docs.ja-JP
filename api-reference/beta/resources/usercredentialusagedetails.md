---
title: Usercredential使い方の詳細リソースの種類
description: 指定したテナントのセルフサービスによるパスワードのリセットの使用法を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: bb92f3bfc91e8fa418d6a33ad6a77a5fddbf9f10
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527631"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="e08e7-103">Usercredential使い方の詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e08e7-103">userCredentialUsageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e08e7-104">指定したテナントのセルフサービスによるパスワードのリセットの使用法を表します。</span><span class="sxs-lookup"><span data-stu-id="e08e7-104">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="e08e7-105">詳細には、ユーザー情報、リセットの状態、およびエラーの理由が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e08e7-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="e08e7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e08e7-106">Methods</span></span>

| <span data-ttu-id="e08e7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e08e7-107">Method</span></span>       | <span data-ttu-id="e08e7-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e08e7-108">Return Type</span></span> | <span data-ttu-id="e08e7-109">説明</span><span class="sxs-lookup"><span data-stu-id="e08e7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e08e7-110">Usercredentialの詳細を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e08e7-110">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="e08e7-111">Usercredentialの詳細</span><span class="sxs-lookup"><span data-stu-id="e08e7-111">userCredentialUsageDetails</span></span> | <span data-ttu-id="e08e7-112">Usercredentialの詳細オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e08e7-112">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e08e7-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e08e7-113">Properties</span></span>

| <span data-ttu-id="e08e7-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e08e7-114">Property</span></span>     | <span data-ttu-id="e08e7-115">型</span><span class="sxs-lookup"><span data-stu-id="e08e7-115">Type</span></span>        | <span data-ttu-id="e08e7-116">説明</span><span class="sxs-lookup"><span data-stu-id="e08e7-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e08e7-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="e08e7-117">authMethod</span></span> | <span data-ttu-id="e08e7-118">string</span><span class="sxs-lookup"><span data-stu-id="e08e7-118">string</span></span> | <span data-ttu-id="e08e7-119">ユーザーが使用した認証方法を表します。</span><span class="sxs-lookup"><span data-stu-id="e08e7-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="e08e7-120">可能な値は`email`、 `mobileSMS` `mobileCall`、、 `officePhone`、 `securityQuestion` 、(セルフサービスのパスワードのリセットにのみ使用`appNotification`) `appCode`、、 `alternateMobileCall` 、および (登録でのみサポートされます) です。</span><span class="sxs-lookup"><span data-stu-id="e08e7-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="e08e7-121">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e08e7-121">eventDateTime</span></span> | <span data-ttu-id="e08e7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e08e7-122">DateTimeOffset</span></span> | <span data-ttu-id="e08e7-123">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="e08e7-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e08e7-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e08e7-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="e08e7-125">failureReason</span><span class="sxs-lookup"><span data-stu-id="e08e7-125">failureReason</span></span> | <span data-ttu-id="e08e7-126">String</span><span class="sxs-lookup"><span data-stu-id="e08e7-126">String</span></span> | <span data-ttu-id="e08e7-127">対応するリセットまたは登録ワークフローのエラーの理由を示します。</span><span class="sxs-lookup"><span data-stu-id="e08e7-127">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="e08e7-128">特徴</span><span class="sxs-lookup"><span data-stu-id="e08e7-128">feature</span></span> | <span data-ttu-id="e08e7-129">string</span><span class="sxs-lookup"><span data-stu-id="e08e7-129">string</span></span> | <span data-ttu-id="e08e7-130">可能な値は`registration` 、 `reset`とです。</span><span class="sxs-lookup"><span data-stu-id="e08e7-130">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="e08e7-131">id</span><span class="sxs-lookup"><span data-stu-id="e08e7-131">id</span></span> | <span data-ttu-id="e08e7-132">String</span><span class="sxs-lookup"><span data-stu-id="e08e7-132">String</span></span> | <span data-ttu-id="e08e7-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e08e7-133">Read-only.</span></span> <span data-ttu-id="e08e7-134">アクティビティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e08e7-134">The unique identifier for the activity.</span></span> <span data-ttu-id="e08e7-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e08e7-135">Read-only.</span></span>|
| <span data-ttu-id="e08e7-136">この</span><span class="sxs-lookup"><span data-stu-id="e08e7-136">isSuccess</span></span> | <span data-ttu-id="e08e7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e08e7-137">Boolean</span></span> | <span data-ttu-id="e08e7-138">ワークフローの成功または失敗を示します。</span><span class="sxs-lookup"><span data-stu-id="e08e7-138">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="e08e7-139">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e08e7-139">userDisplayName</span></span> | <span data-ttu-id="e08e7-140">String</span><span class="sxs-lookup"><span data-stu-id="e08e7-140">String</span></span> | <span data-ttu-id="e08e7-141">リセットまたは登録ワークフローを実行するユーザーのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="e08e7-141">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="e08e7-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e08e7-142">userPrincipalName</span></span> | <span data-ttu-id="e08e7-143">String</span><span class="sxs-lookup"><span data-stu-id="e08e7-143">String</span></span> | <span data-ttu-id="e08e7-144">リセットまたは登録ワークフローを実行するユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="e08e7-144">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e08e7-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e08e7-145">Relationships</span></span>

<span data-ttu-id="e08e7-146">なし。</span><span class="sxs-lookup"><span data-stu-id="e08e7-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e08e7-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e08e7-147">JSON representation</span></span>

<span data-ttu-id="e08e7-148">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e08e7-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->