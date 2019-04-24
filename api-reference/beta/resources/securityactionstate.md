---
title: securityactionstate リソースの種類
description: securityAction 状態の変更履歴を表します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8f789dab438316f16b9c2607947fa08b7fcefdc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522021"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="7b678-103">securityactionstate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b678-103">securityActionState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b678-104">securityAction 状態の変更履歴を表します。</span><span class="sxs-lookup"><span data-stu-id="7b678-104">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="7b678-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b678-105">Properties</span></span>

| <span data-ttu-id="7b678-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b678-106">Property</span></span>     | <span data-ttu-id="7b678-107">型</span><span class="sxs-lookup"><span data-stu-id="7b678-107">Type</span></span>        | <span data-ttu-id="7b678-108">説明</span><span class="sxs-lookup"><span data-stu-id="7b678-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b678-109">appId</span><span class="sxs-lookup"><span data-stu-id="7b678-109">appId</span></span>|<span data-ttu-id="7b678-110">String</span><span class="sxs-lookup"><span data-stu-id="7b678-110">String</span></span>|<span data-ttu-id="7b678-111">アクションに更新プログラム (PATCH) を送信した、呼び出し元アプリケーションのアプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="7b678-111">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="7b678-112">は`appId` 、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="7b678-112">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="7b678-113">status</span><span class="sxs-lookup"><span data-stu-id="7b678-113">status</span></span>|<span data-ttu-id="7b678-114">String</span><span class="sxs-lookup"><span data-stu-id="7b678-114">String</span></span>| <span data-ttu-id="7b678-115">この更新プログラムの securityAction の状態。</span><span class="sxs-lookup"><span data-stu-id="7b678-115">Status of the securityAction in this update.</span></span> <span data-ttu-id="7b678-116">可能な値は、`NotStarted`、`Running`、`Completed`、`Failed` です。</span><span class="sxs-lookup"><span data-stu-id="7b678-116">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="7b678-117">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b678-117">updatedDateTime</span></span>|<span data-ttu-id="7b678-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b678-118">DateTimeOffset</span></span>| <span data-ttu-id="7b678-119">actionstate が更新されたときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="7b678-119">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="7b678-120">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7b678-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7b678-121">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7b678-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7b678-122">user</span><span class="sxs-lookup"><span data-stu-id="7b678-122">user</span></span>|<span data-ttu-id="7b678-123">String</span><span class="sxs-lookup"><span data-stu-id="7b678-123">String</span></span>|<span data-ttu-id="7b678-124">更新 (PATCH) をアクションに送信した、サインインしているユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="7b678-124">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="7b678-125">は`user` 、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="7b678-125">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b678-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b678-126">JSON representation</span></span>

<span data-ttu-id="7b678-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b678-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
