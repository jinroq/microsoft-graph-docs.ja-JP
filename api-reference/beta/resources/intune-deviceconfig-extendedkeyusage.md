---
title: extendedkeyusage リソースの種類
description: カスタム拡張キー使用法の定義
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd89a46c2739f80a0a5c661884fb5e72c6e17522
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789214"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="4a615-103">extendedkeyusage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a615-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="4a615-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a615-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a615-106">カスタム拡張キー使用法の定義</span><span class="sxs-lookup"><span data-stu-id="4a615-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="4a615-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a615-107">Properties</span></span>
|<span data-ttu-id="4a615-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a615-108">Property</span></span>|<span data-ttu-id="4a615-109">型</span><span class="sxs-lookup"><span data-stu-id="4a615-109">Type</span></span>|<span data-ttu-id="4a615-110">説明</span><span class="sxs-lookup"><span data-stu-id="4a615-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a615-111">name</span><span class="sxs-lookup"><span data-stu-id="4a615-111">name</span></span>|<span data-ttu-id="4a615-112">String</span><span class="sxs-lookup"><span data-stu-id="4a615-112">String</span></span>|<span data-ttu-id="4a615-113">拡張キー使用法の名前</span><span class="sxs-lookup"><span data-stu-id="4a615-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="4a615-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a615-114">objectIdentifier</span></span>|<span data-ttu-id="4a615-115">文字列</span><span class="sxs-lookup"><span data-stu-id="4a615-115">String</span></span>|<span data-ttu-id="4a615-116">拡張キー使用法のオブジェクト識別子</span><span class="sxs-lookup"><span data-stu-id="4a615-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a615-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4a615-117">Relationships</span></span>
<span data-ttu-id="4a615-118">なし</span><span class="sxs-lookup"><span data-stu-id="4a615-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a615-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a615-119">JSON Representation</span></span>
<span data-ttu-id="4a615-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4a615-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





