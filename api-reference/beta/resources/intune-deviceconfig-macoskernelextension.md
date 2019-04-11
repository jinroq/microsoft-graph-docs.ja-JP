---
title: macOSKernelExtension リソースの種類
description: 特定の macOS カーネル拡張情報を表します。 macOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04320f92045ae128ca1bf128484d2aa55f03d706
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808954"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="1832c-104">macOSKernelExtension リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1832c-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="1832c-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1832c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1832c-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1832c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1832c-107">特定の macOS カーネル拡張情報を表します。</span><span class="sxs-lookup"><span data-stu-id="1832c-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="1832c-108">macOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。</span><span class="sxs-lookup"><span data-stu-id="1832c-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="1832c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1832c-109">Properties</span></span>
|<span data-ttu-id="1832c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1832c-110">Property</span></span>|<span data-ttu-id="1832c-111">型</span><span class="sxs-lookup"><span data-stu-id="1832c-111">Type</span></span>|<span data-ttu-id="1832c-112">説明</span><span class="sxs-lookup"><span data-stu-id="1832c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1832c-113">teamidentifier</span><span class="sxs-lookup"><span data-stu-id="1832c-113">teamIdentifier</span></span>|<span data-ttu-id="1832c-114">文字列</span><span class="sxs-lookup"><span data-stu-id="1832c-114">String</span></span>|<span data-ttu-id="1832c-115">カーネル拡張機能の署名に使用されたチーム識別子。</span><span class="sxs-lookup"><span data-stu-id="1832c-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="1832c-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="1832c-116">bundleId</span></span>|<span data-ttu-id="1832c-117">String</span><span class="sxs-lookup"><span data-stu-id="1832c-117">String</span></span>|<span data-ttu-id="1832c-118">カーネル拡張機能のバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="1832c-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1832c-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1832c-119">Relationships</span></span>
<span data-ttu-id="1832c-120">なし</span><span class="sxs-lookup"><span data-stu-id="1832c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1832c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1832c-121">JSON Representation</span></span>
<span data-ttu-id="1832c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1832c-122">Here is a JSON representation of the resource.</span></span>
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





