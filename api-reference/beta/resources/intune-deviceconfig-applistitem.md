---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7e005681917f0edffe00b33947d2bd2bd5b2ff5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172248"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="9cbb9-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9cbb9-103">appListItem resource type</span></span>

> <span data-ttu-id="9cbb9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cbb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cbb9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9cbb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cbb9-106">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="9cbb9-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="9cbb9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cbb9-107">Properties</span></span>
|<span data-ttu-id="9cbb9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cbb9-108">Property</span></span>|<span data-ttu-id="9cbb9-109">型</span><span class="sxs-lookup"><span data-stu-id="9cbb9-109">Type</span></span>|<span data-ttu-id="9cbb9-110">説明</span><span class="sxs-lookup"><span data-stu-id="9cbb9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cbb9-111">name</span><span class="sxs-lookup"><span data-stu-id="9cbb9-111">name</span></span>|<span data-ttu-id="9cbb9-112">String</span><span class="sxs-lookup"><span data-stu-id="9cbb9-112">String</span></span>|<span data-ttu-id="9cbb9-113">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="9cbb9-113">The application name</span></span>|
|<span data-ttu-id="9cbb9-114">発行元</span><span class="sxs-lookup"><span data-stu-id="9cbb9-114">publisher</span></span>|<span data-ttu-id="9cbb9-115">String</span><span class="sxs-lookup"><span data-stu-id="9cbb9-115">String</span></span>|<span data-ttu-id="9cbb9-116">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="9cbb9-116">The publisher of the application</span></span>|
|<span data-ttu-id="9cbb9-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9cbb9-117">appStoreUrl</span></span>|<span data-ttu-id="9cbb9-118">String</span><span class="sxs-lookup"><span data-stu-id="9cbb9-118">String</span></span>|<span data-ttu-id="9cbb9-119">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="9cbb9-119">The Store URL of the application</span></span>|
|<span data-ttu-id="9cbb9-120">appId</span><span class="sxs-lookup"><span data-stu-id="9cbb9-120">appId</span></span>|<span data-ttu-id="9cbb9-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9cbb9-121">String</span></span>|<span data-ttu-id="9cbb9-122">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="9cbb9-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cbb9-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9cbb9-123">Relationships</span></span>
<span data-ttu-id="9cbb9-124">なし</span><span class="sxs-lookup"><span data-stu-id="9cbb9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cbb9-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9cbb9-125">JSON Representation</span></span>
<span data-ttu-id="9cbb9-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9cbb9-126">Here is a JSON representation of the resource.</span></span>
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




