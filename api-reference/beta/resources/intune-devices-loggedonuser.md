---
title: loggedOnUser リソースの種類
description: ログオンユーザー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5dfaa8bbaa879fc48c5f6ea31d1b7b14e998820
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148931"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="e0d96-103">loggedOnUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0d96-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="e0d96-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0d96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0d96-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0d96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0d96-106">ログオンユーザー</span><span class="sxs-lookup"><span data-stu-id="e0d96-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="e0d96-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0d96-107">Properties</span></span>
|<span data-ttu-id="e0d96-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0d96-108">Property</span></span>|<span data-ttu-id="e0d96-109">型</span><span class="sxs-lookup"><span data-stu-id="e0d96-109">Type</span></span>|<span data-ttu-id="e0d96-110">説明</span><span class="sxs-lookup"><span data-stu-id="e0d96-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0d96-111">userId</span><span class="sxs-lookup"><span data-stu-id="e0d96-111">userId</span></span>|<span data-ttu-id="e0d96-112">String</span><span class="sxs-lookup"><span data-stu-id="e0d96-112">String</span></span>|<span data-ttu-id="e0d96-113">ユーザー id</span><span class="sxs-lookup"><span data-stu-id="e0d96-113">User id</span></span>|
|<span data-ttu-id="e0d96-114">lastlogondatetime</span><span class="sxs-lookup"><span data-stu-id="e0d96-114">lastLogOnDateTime</span></span>|<span data-ttu-id="e0d96-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0d96-115">DateTimeOffset</span></span>|<span data-ttu-id="e0d96-116">ユーザーがログオンした日時</span><span class="sxs-lookup"><span data-stu-id="e0d96-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0d96-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0d96-117">Relationships</span></span>
<span data-ttu-id="e0d96-118">なし</span><span class="sxs-lookup"><span data-stu-id="e0d96-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0d96-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0d96-119">JSON Representation</span></span>
<span data-ttu-id="e0d96-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0d96-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




