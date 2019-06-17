---
title: macOSKernelExtension リソースの種類
description: 特定の macOS カーネル拡張情報を表します。 MacOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52b552b0817207968c0a0ab7bb9dcc9bab0a4f44
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992179"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="013d8-104">macOSKernelExtension リソースの種類</span><span class="sxs-lookup"><span data-stu-id="013d8-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="013d8-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="013d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="013d8-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="013d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="013d8-107">特定の macOS カーネル拡張情報を表します。</span><span class="sxs-lookup"><span data-stu-id="013d8-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="013d8-108">MacOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。</span><span class="sxs-lookup"><span data-stu-id="013d8-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="013d8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="013d8-109">Properties</span></span>
|<span data-ttu-id="013d8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="013d8-110">Property</span></span>|<span data-ttu-id="013d8-111">型</span><span class="sxs-lookup"><span data-stu-id="013d8-111">Type</span></span>|<span data-ttu-id="013d8-112">説明</span><span class="sxs-lookup"><span data-stu-id="013d8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="013d8-113">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="013d8-113">teamIdentifier</span></span>|<span data-ttu-id="013d8-114">String</span><span class="sxs-lookup"><span data-stu-id="013d8-114">String</span></span>|<span data-ttu-id="013d8-115">カーネル拡張機能の署名に使用されたチーム識別子。</span><span class="sxs-lookup"><span data-stu-id="013d8-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="013d8-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="013d8-116">bundleId</span></span>|<span data-ttu-id="013d8-117">String</span><span class="sxs-lookup"><span data-stu-id="013d8-117">String</span></span>|<span data-ttu-id="013d8-118">カーネル拡張機能のバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="013d8-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="013d8-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="013d8-119">Relationships</span></span>
<span data-ttu-id="013d8-120">なし</span><span class="sxs-lookup"><span data-stu-id="013d8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="013d8-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="013d8-121">JSON Representation</span></span>
<span data-ttu-id="013d8-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="013d8-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```





