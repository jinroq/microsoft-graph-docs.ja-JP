---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b9aa0a35767078b7c91f72b7a8b06a450cc9f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028610"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="bbece-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bbece-103">appListItem resource type</span></span>

> <span data-ttu-id="bbece-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bbece-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbece-105">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="bbece-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="bbece-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbece-106">Properties</span></span>
|<span data-ttu-id="bbece-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbece-107">Property</span></span>|<span data-ttu-id="bbece-108">型</span><span class="sxs-lookup"><span data-stu-id="bbece-108">Type</span></span>|<span data-ttu-id="bbece-109">説明</span><span class="sxs-lookup"><span data-stu-id="bbece-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbece-110">name</span><span class="sxs-lookup"><span data-stu-id="bbece-110">name</span></span>|<span data-ttu-id="bbece-111">String</span><span class="sxs-lookup"><span data-stu-id="bbece-111">String</span></span>|<span data-ttu-id="bbece-112">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="bbece-112">The application name</span></span>|
|<span data-ttu-id="bbece-113">発行元</span><span class="sxs-lookup"><span data-stu-id="bbece-113">publisher</span></span>|<span data-ttu-id="bbece-114">String</span><span class="sxs-lookup"><span data-stu-id="bbece-114">String</span></span>|<span data-ttu-id="bbece-115">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="bbece-115">The publisher of the application</span></span>|
|<span data-ttu-id="bbece-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bbece-116">appStoreUrl</span></span>|<span data-ttu-id="bbece-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bbece-117">String</span></span>|<span data-ttu-id="bbece-118">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="bbece-118">The Store URL of the application</span></span>|
|<span data-ttu-id="bbece-119">appId</span><span class="sxs-lookup"><span data-stu-id="bbece-119">appId</span></span>|<span data-ttu-id="bbece-120">String</span><span class="sxs-lookup"><span data-stu-id="bbece-120">String</span></span>|<span data-ttu-id="bbece-121">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="bbece-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbece-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bbece-122">Relationships</span></span>
<span data-ttu-id="bbece-123">なし</span><span class="sxs-lookup"><span data-stu-id="bbece-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbece-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbece-124">JSON Representation</span></span>
<span data-ttu-id="bbece-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bbece-125">Here is a JSON representation of the resource.</span></span>
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



