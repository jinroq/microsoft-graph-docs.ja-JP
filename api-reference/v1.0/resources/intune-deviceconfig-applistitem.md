---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253079"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="f8313-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f8313-103">appListItem resource type</span></span>

> <span data-ttu-id="f8313-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f8313-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8313-105">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="f8313-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="f8313-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8313-106">Properties</span></span>
|<span data-ttu-id="f8313-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8313-107">Property</span></span>|<span data-ttu-id="f8313-108">型</span><span class="sxs-lookup"><span data-stu-id="f8313-108">Type</span></span>|<span data-ttu-id="f8313-109">説明</span><span class="sxs-lookup"><span data-stu-id="f8313-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8313-110">name</span><span class="sxs-lookup"><span data-stu-id="f8313-110">name</span></span>|<span data-ttu-id="f8313-111">String</span><span class="sxs-lookup"><span data-stu-id="f8313-111">String</span></span>|<span data-ttu-id="f8313-112">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="f8313-112">The application name</span></span>|
|<span data-ttu-id="f8313-113">発行元</span><span class="sxs-lookup"><span data-stu-id="f8313-113">publisher</span></span>|<span data-ttu-id="f8313-114">String</span><span class="sxs-lookup"><span data-stu-id="f8313-114">String</span></span>|<span data-ttu-id="f8313-115">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="f8313-115">The publisher of the application</span></span>|
|<span data-ttu-id="f8313-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f8313-116">appStoreUrl</span></span>|<span data-ttu-id="f8313-117">String</span><span class="sxs-lookup"><span data-stu-id="f8313-117">String</span></span>|<span data-ttu-id="f8313-118">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="f8313-118">The Store URL of the application</span></span>|
|<span data-ttu-id="f8313-119">appId</span><span class="sxs-lookup"><span data-stu-id="f8313-119">appId</span></span>|<span data-ttu-id="f8313-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f8313-120">String</span></span>|<span data-ttu-id="f8313-121">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="f8313-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8313-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f8313-122">Relationships</span></span>
<span data-ttu-id="f8313-123">なし</span><span class="sxs-lookup"><span data-stu-id="f8313-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8313-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8313-124">JSON Representation</span></span>
<span data-ttu-id="f8313-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f8313-125">Here is a JSON representation of the resource.</span></span>
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



