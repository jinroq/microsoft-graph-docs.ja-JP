---
title: macOSKernelExtension リソースの種類
description: 特定の macOS カーネル拡張情報を表します。 macOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04320f92045ae128ca1bf128484d2aa55f03d706
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570646"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="a7be5-104">macOSKernelExtension リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7be5-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="a7be5-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7be5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7be5-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7be5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7be5-107">特定の macOS カーネル拡張情報を表します。</span><span class="sxs-lookup"><span data-stu-id="a7be5-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="a7be5-108">macOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。</span><span class="sxs-lookup"><span data-stu-id="a7be5-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="a7be5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7be5-109">Properties</span></span>
|<span data-ttu-id="a7be5-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7be5-110">Property</span></span>|<span data-ttu-id="a7be5-111">型</span><span class="sxs-lookup"><span data-stu-id="a7be5-111">Type</span></span>|<span data-ttu-id="a7be5-112">説明</span><span class="sxs-lookup"><span data-stu-id="a7be5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7be5-113">teamidentifier</span><span class="sxs-lookup"><span data-stu-id="a7be5-113">teamIdentifier</span></span>|<span data-ttu-id="a7be5-114">String</span><span class="sxs-lookup"><span data-stu-id="a7be5-114">String</span></span>|<span data-ttu-id="a7be5-115">カーネル拡張機能の署名に使用されたチーム識別子。</span><span class="sxs-lookup"><span data-stu-id="a7be5-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="a7be5-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="a7be5-116">bundleId</span></span>|<span data-ttu-id="a7be5-117">String</span><span class="sxs-lookup"><span data-stu-id="a7be5-117">String</span></span>|<span data-ttu-id="a7be5-118">カーネル拡張機能のバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="a7be5-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7be5-119">関係</span><span class="sxs-lookup"><span data-stu-id="a7be5-119">Relationships</span></span>
<span data-ttu-id="a7be5-120">なし</span><span class="sxs-lookup"><span data-stu-id="a7be5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7be5-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7be5-121">JSON Representation</span></span>
<span data-ttu-id="a7be5-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7be5-122">Here is a JSON representation of the resource.</span></span>
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





