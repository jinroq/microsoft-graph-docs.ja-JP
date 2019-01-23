---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9571b622fc098f384f7c3a6c62b1d1e10d89f663
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405416"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="50423-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50423-103">appListItem resource type</span></span>

> <span data-ttu-id="50423-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="50423-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50423-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50423-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50423-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50423-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50423-107">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="50423-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="50423-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50423-108">Properties</span></span>
|<span data-ttu-id="50423-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50423-109">Property</span></span>|<span data-ttu-id="50423-110">型</span><span class="sxs-lookup"><span data-stu-id="50423-110">Type</span></span>|<span data-ttu-id="50423-111">説明</span><span class="sxs-lookup"><span data-stu-id="50423-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50423-112">name</span><span class="sxs-lookup"><span data-stu-id="50423-112">name</span></span>|<span data-ttu-id="50423-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="50423-113">String</span></span>|<span data-ttu-id="50423-114">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="50423-114">The application name</span></span>|
|<span data-ttu-id="50423-115">発行元</span><span class="sxs-lookup"><span data-stu-id="50423-115">publisher</span></span>|<span data-ttu-id="50423-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="50423-116">String</span></span>|<span data-ttu-id="50423-117">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="50423-117">The publisher of the application</span></span>|
|<span data-ttu-id="50423-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="50423-118">appStoreUrl</span></span>|<span data-ttu-id="50423-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="50423-119">String</span></span>|<span data-ttu-id="50423-120">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="50423-120">The Store URL of the application</span></span>|
|<span data-ttu-id="50423-121">appId</span><span class="sxs-lookup"><span data-stu-id="50423-121">appId</span></span>|<span data-ttu-id="50423-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="50423-122">String</span></span>|<span data-ttu-id="50423-123">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="50423-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="50423-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="50423-124">Relationships</span></span>
<span data-ttu-id="50423-125">なし</span><span class="sxs-lookup"><span data-stu-id="50423-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50423-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50423-126">JSON Representation</span></span>
<span data-ttu-id="50423-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="50423-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




