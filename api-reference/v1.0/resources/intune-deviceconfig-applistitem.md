---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575094"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="fa04e-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa04e-103">appListItem resource type</span></span>

> <span data-ttu-id="fa04e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa04e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa04e-105">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="fa04e-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="fa04e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa04e-106">Properties</span></span>
|<span data-ttu-id="fa04e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa04e-107">Property</span></span>|<span data-ttu-id="fa04e-108">型</span><span class="sxs-lookup"><span data-stu-id="fa04e-108">Type</span></span>|<span data-ttu-id="fa04e-109">説明</span><span class="sxs-lookup"><span data-stu-id="fa04e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa04e-110">name</span><span class="sxs-lookup"><span data-stu-id="fa04e-110">name</span></span>|<span data-ttu-id="fa04e-111">String</span><span class="sxs-lookup"><span data-stu-id="fa04e-111">String</span></span>|<span data-ttu-id="fa04e-112">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="fa04e-112">The application name</span></span>|
|<span data-ttu-id="fa04e-113">発行元</span><span class="sxs-lookup"><span data-stu-id="fa04e-113">publisher</span></span>|<span data-ttu-id="fa04e-114">String</span><span class="sxs-lookup"><span data-stu-id="fa04e-114">String</span></span>|<span data-ttu-id="fa04e-115">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="fa04e-115">The publisher of the application</span></span>|
|<span data-ttu-id="fa04e-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="fa04e-116">appStoreUrl</span></span>|<span data-ttu-id="fa04e-117">String</span><span class="sxs-lookup"><span data-stu-id="fa04e-117">String</span></span>|<span data-ttu-id="fa04e-118">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="fa04e-118">The Store URL of the application</span></span>|
|<span data-ttu-id="fa04e-119">appId</span><span class="sxs-lookup"><span data-stu-id="fa04e-119">appId</span></span>|<span data-ttu-id="fa04e-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fa04e-120">String</span></span>|<span data-ttu-id="fa04e-121">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="fa04e-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa04e-122">関係</span><span class="sxs-lookup"><span data-stu-id="fa04e-122">Relationships</span></span>
<span data-ttu-id="fa04e-123">なし</span><span class="sxs-lookup"><span data-stu-id="fa04e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa04e-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa04e-124">JSON Representation</span></span>
<span data-ttu-id="fa04e-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa04e-125">Here is a JSON representation of the resource.</span></span>
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



