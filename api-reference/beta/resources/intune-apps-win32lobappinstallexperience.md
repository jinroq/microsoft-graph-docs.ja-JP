---
title: win32LobAppInstallExperience リソースの種類
description: Win32 アプリのインストール環境のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8cb0efbec4044bb63b9c8069e12bf934662ca587
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335670"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="da0a2-103">win32LobAppInstallExperience リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da0a2-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="da0a2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da0a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da0a2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da0a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da0a2-106">Win32 アプリのインストール環境のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="da0a2-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="da0a2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da0a2-107">Properties</span></span>
|<span data-ttu-id="da0a2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da0a2-108">Property</span></span>|<span data-ttu-id="da0a2-109">型</span><span class="sxs-lookup"><span data-stu-id="da0a2-109">Type</span></span>|<span data-ttu-id="da0a2-110">説明</span><span class="sxs-lookup"><span data-stu-id="da0a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da0a2-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="da0a2-111">runAsAccount</span></span>|[<span data-ttu-id="da0a2-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="da0a2-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="da0a2-113">アプリが実行されている実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="da0a2-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="da0a2-114">可能な値: `system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="da0a2-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da0a2-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da0a2-115">Relationships</span></span>
<span data-ttu-id="da0a2-116">なし</span><span class="sxs-lookup"><span data-stu-id="da0a2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da0a2-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da0a2-117">JSON Representation</span></span>
<span data-ttu-id="da0a2-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="da0a2-118">Here is a JSON representation of the resource.</span></span>
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



