---
title: macOSKernelExtension リソースの種類
description: 特定の macOS カーネル拡張情報を表します。 MacOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fbf12bd16bdf606010bc9b6518c8241fe28eb765
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321933"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="c95c7-104">macOSKernelExtension リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c95c7-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="c95c7-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c95c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c95c7-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c95c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c95c7-107">特定の macOS カーネル拡張情報を表します。</span><span class="sxs-lookup"><span data-stu-id="c95c7-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="c95c7-108">MacOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。</span><span class="sxs-lookup"><span data-stu-id="c95c7-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="c95c7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c95c7-109">Properties</span></span>
|<span data-ttu-id="c95c7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c95c7-110">Property</span></span>|<span data-ttu-id="c95c7-111">型</span><span class="sxs-lookup"><span data-stu-id="c95c7-111">Type</span></span>|<span data-ttu-id="c95c7-112">説明</span><span class="sxs-lookup"><span data-stu-id="c95c7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c95c7-113">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="c95c7-113">teamIdentifier</span></span>|<span data-ttu-id="c95c7-114">String</span><span class="sxs-lookup"><span data-stu-id="c95c7-114">String</span></span>|<span data-ttu-id="c95c7-115">カーネル拡張機能の署名に使用されたチーム識別子。</span><span class="sxs-lookup"><span data-stu-id="c95c7-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="c95c7-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="c95c7-116">bundleId</span></span>|<span data-ttu-id="c95c7-117">String</span><span class="sxs-lookup"><span data-stu-id="c95c7-117">String</span></span>|<span data-ttu-id="c95c7-118">カーネル拡張機能のバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="c95c7-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c95c7-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c95c7-119">Relationships</span></span>
<span data-ttu-id="c95c7-120">なし</span><span class="sxs-lookup"><span data-stu-id="c95c7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c95c7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c95c7-121">JSON Representation</span></span>
<span data-ttu-id="c95c7-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c95c7-122">Here is a JSON representation of the resource.</span></span>
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



