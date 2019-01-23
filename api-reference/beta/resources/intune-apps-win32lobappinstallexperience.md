---
title: win32LobAppInstallExperience リソースの種類
description: Win32 アプリケーションのインストール環境のプロパティが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 240000dfceaa2ef4e973167cbd3b5a743d346892
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406690"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="27943-103">win32LobAppInstallExperience リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27943-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="27943-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27943-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27943-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27943-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27943-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27943-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27943-107">Win32 アプリケーションのインストール環境のプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="27943-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="27943-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27943-108">Properties</span></span>
|<span data-ttu-id="27943-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27943-109">Property</span></span>|<span data-ttu-id="27943-110">型</span><span class="sxs-lookup"><span data-stu-id="27943-110">Type</span></span>|<span data-ttu-id="27943-111">説明</span><span class="sxs-lookup"><span data-stu-id="27943-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27943-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="27943-112">runAsAccount</span></span>|[<span data-ttu-id="27943-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="27943-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="27943-114">アプリケーションが実行される実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="27943-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="27943-115">可能な値: `system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="27943-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27943-116">関係</span><span class="sxs-lookup"><span data-stu-id="27943-116">Relationships</span></span>
<span data-ttu-id="27943-117">なし</span><span class="sxs-lookup"><span data-stu-id="27943-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27943-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27943-118">JSON Representation</span></span>
<span data-ttu-id="27943-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="27943-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```




