---
title: win32LobAppReturnCode リソースの種類
description: Win32 アプリケーションのプロパティ戻り値のコードにはが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e6357d0ac6aab87e236e02d60454d1b45aa98fe1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404359"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="cf6eb-103">win32LobAppReturnCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf6eb-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="cf6eb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf6eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf6eb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf6eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf6eb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf6eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf6eb-107">Win32 アプリケーションのプロパティ戻り値のコードにはが含まれています</span><span class="sxs-lookup"><span data-stu-id="cf6eb-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="cf6eb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf6eb-108">Properties</span></span>
|<span data-ttu-id="cf6eb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf6eb-109">Property</span></span>|<span data-ttu-id="cf6eb-110">型</span><span class="sxs-lookup"><span data-stu-id="cf6eb-110">Type</span></span>|<span data-ttu-id="cf6eb-111">説明</span><span class="sxs-lookup"><span data-stu-id="cf6eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf6eb-112">リターン コード</span><span class="sxs-lookup"><span data-stu-id="cf6eb-112">returnCode</span></span>|<span data-ttu-id="cf6eb-113">Int32</span><span class="sxs-lookup"><span data-stu-id="cf6eb-113">Int32</span></span>|<span data-ttu-id="cf6eb-114">コードを返します。</span><span class="sxs-lookup"><span data-stu-id="cf6eb-114">Return code.</span></span>|
|<span data-ttu-id="cf6eb-115">type</span><span class="sxs-lookup"><span data-stu-id="cf6eb-115">type</span></span>|[<span data-ttu-id="cf6eb-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="cf6eb-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="cf6eb-117">コードの戻り値の型。</span><span class="sxs-lookup"><span data-stu-id="cf6eb-117">The type of return code.</span></span> <span data-ttu-id="cf6eb-118">可能な値は、`failed`、`success`、`softReboot`、`hardReboot`、`retry` です。</span><span class="sxs-lookup"><span data-stu-id="cf6eb-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf6eb-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf6eb-119">Relationships</span></span>
<span data-ttu-id="cf6eb-120">なし</span><span class="sxs-lookup"><span data-stu-id="cf6eb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf6eb-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf6eb-121">JSON Representation</span></span>
<span data-ttu-id="cf6eb-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf6eb-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```




