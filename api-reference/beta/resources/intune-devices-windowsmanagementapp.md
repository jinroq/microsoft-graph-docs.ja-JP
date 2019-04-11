---
title: windowsmanagementapp リソースの種類
description: Windows management app エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99367ae51bbfe2ad044a99b465f70f5f8316e2d8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802423"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="bc39d-103">windowsmanagementapp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc39d-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="bc39d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc39d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc39d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc39d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc39d-106">Windows management app エンティティ。</span><span class="sxs-lookup"><span data-stu-id="bc39d-106">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="bc39d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc39d-107">Methods</span></span>
|<span data-ttu-id="bc39d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc39d-108">Method</span></span>|<span data-ttu-id="bc39d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bc39d-109">Return Type</span></span>|<span data-ttu-id="bc39d-110">説明</span><span class="sxs-lookup"><span data-stu-id="bc39d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc39d-111">windowsmanagementapp の取得</span><span class="sxs-lookup"><span data-stu-id="bc39d-111">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="bc39d-112">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="bc39d-112">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="bc39d-113">[windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bc39d-113">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="bc39d-114">windowsmanagementapp の更新</span><span class="sxs-lookup"><span data-stu-id="bc39d-114">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="bc39d-115">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="bc39d-115">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="bc39d-116">[windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc39d-116">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc39d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc39d-117">Properties</span></span>
|<span data-ttu-id="bc39d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc39d-118">Property</span></span>|<span data-ttu-id="bc39d-119">型</span><span class="sxs-lookup"><span data-stu-id="bc39d-119">Type</span></span>|<span data-ttu-id="bc39d-120">説明</span><span class="sxs-lookup"><span data-stu-id="bc39d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc39d-121">id</span><span class="sxs-lookup"><span data-stu-id="bc39d-121">id</span></span>|<span data-ttu-id="bc39d-122">String</span><span class="sxs-lookup"><span data-stu-id="bc39d-122">String</span></span>|<span data-ttu-id="bc39d-123">Windows management アプリの一意識別子</span><span class="sxs-lookup"><span data-stu-id="bc39d-123">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="bc39d-124">プロパティ availableversion</span><span class="sxs-lookup"><span data-stu-id="bc39d-124">availableVersion</span></span>|<span data-ttu-id="bc39d-125">文字列</span><span class="sxs-lookup"><span data-stu-id="bc39d-125">String</span></span>|<span data-ttu-id="bc39d-126">Windows management アプリの利用可能なバージョン。</span><span class="sxs-lookup"><span data-stu-id="bc39d-126">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc39d-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc39d-127">Relationships</span></span>
|<span data-ttu-id="bc39d-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc39d-128">Relationship</span></span>|<span data-ttu-id="bc39d-129">型</span><span class="sxs-lookup"><span data-stu-id="bc39d-129">Type</span></span>|<span data-ttu-id="bc39d-130">説明</span><span class="sxs-lookup"><span data-stu-id="bc39d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc39d-131">healthSummary</span><span class="sxs-lookup"><span data-stu-id="bc39d-131">healthSummary</span></span>|[<span data-ttu-id="bc39d-132">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="bc39d-132">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="bc39d-133">Windows management アプリの正常性の概要。</span><span class="sxs-lookup"><span data-stu-id="bc39d-133">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="bc39d-134">healthStates</span><span class="sxs-lookup"><span data-stu-id="bc39d-134">healthStates</span></span>|<span data-ttu-id="bc39d-135">[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bc39d-135">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="bc39d-136">インストールされている Windows management アプリの正常性状態の一覧。</span><span class="sxs-lookup"><span data-stu-id="bc39d-136">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc39d-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc39d-137">JSON Representation</span></span>
<span data-ttu-id="bc39d-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc39d-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```





