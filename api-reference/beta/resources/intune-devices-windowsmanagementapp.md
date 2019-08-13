---
title: windowsManagementApp リソースの種類
description: Windows management app エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b86d6d6ddad847b1a4b39fd96d61f619e19afaac
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365224"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="653b4-103">windowsManagementApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="653b4-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="653b4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="653b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="653b4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="653b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="653b4-106">Windows management app エンティティ。</span><span class="sxs-lookup"><span data-stu-id="653b4-106">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="653b4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="653b4-107">Methods</span></span>
|<span data-ttu-id="653b4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="653b4-108">Method</span></span>|<span data-ttu-id="653b4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="653b4-109">Return Type</span></span>|<span data-ttu-id="653b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="653b4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="653b4-111">WindowsManagementApp の取得</span><span class="sxs-lookup"><span data-stu-id="653b4-111">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="653b4-112">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="653b4-112">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="653b4-113">[Windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="653b4-113">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="653b4-114">WindowsManagementApp の更新</span><span class="sxs-lookup"><span data-stu-id="653b4-114">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="653b4-115">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="653b4-115">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="653b4-116">[Windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="653b4-116">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="653b4-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="653b4-117">Properties</span></span>
|<span data-ttu-id="653b4-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="653b4-118">Property</span></span>|<span data-ttu-id="653b4-119">型</span><span class="sxs-lookup"><span data-stu-id="653b4-119">Type</span></span>|<span data-ttu-id="653b4-120">説明</span><span class="sxs-lookup"><span data-stu-id="653b4-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="653b4-121">id</span><span class="sxs-lookup"><span data-stu-id="653b4-121">id</span></span>|<span data-ttu-id="653b4-122">String</span><span class="sxs-lookup"><span data-stu-id="653b4-122">String</span></span>|<span data-ttu-id="653b4-123">Windows management アプリの一意識別子</span><span class="sxs-lookup"><span data-stu-id="653b4-123">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="653b4-124">プロパティ availableversion</span><span class="sxs-lookup"><span data-stu-id="653b4-124">availableVersion</span></span>|<span data-ttu-id="653b4-125">String</span><span class="sxs-lookup"><span data-stu-id="653b4-125">String</span></span>|<span data-ttu-id="653b4-126">Windows management アプリの利用可能なバージョン。</span><span class="sxs-lookup"><span data-stu-id="653b4-126">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="653b4-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="653b4-127">Relationships</span></span>
|<span data-ttu-id="653b4-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="653b4-128">Relationship</span></span>|<span data-ttu-id="653b4-129">型</span><span class="sxs-lookup"><span data-stu-id="653b4-129">Type</span></span>|<span data-ttu-id="653b4-130">説明</span><span class="sxs-lookup"><span data-stu-id="653b4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="653b4-131">healthStates</span><span class="sxs-lookup"><span data-stu-id="653b4-131">healthStates</span></span>|<span data-ttu-id="653b4-132">[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="653b4-132">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="653b4-133">インストールされている Windows management アプリの正常性状態の一覧。</span><span class="sxs-lookup"><span data-stu-id="653b4-133">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="653b4-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="653b4-134">JSON Representation</span></span>
<span data-ttu-id="653b4-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="653b4-135">Here is a JSON representation of the resource.</span></span>
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



