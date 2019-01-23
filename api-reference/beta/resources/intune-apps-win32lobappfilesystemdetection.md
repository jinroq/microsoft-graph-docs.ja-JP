---
title: win32LobAppFileSystemDetection リソースの種類
description: Win32 アプリケーションを検出するためにファイルまたはフォルダーのパスが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5fb4e66ce17fb7a964f3210244e2f3a7027c578
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415230"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="707ed-103">win32LobAppFileSystemDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="707ed-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="707ed-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="707ed-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="707ed-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="707ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="707ed-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="707ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="707ed-107">Win32 アプリケーションを検出するためにファイルまたはフォルダーのパスが含まれています</span><span class="sxs-lookup"><span data-stu-id="707ed-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="707ed-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="707ed-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="707ed-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="707ed-109">Properties</span></span>
|<span data-ttu-id="707ed-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="707ed-110">Property</span></span>|<span data-ttu-id="707ed-111">型</span><span class="sxs-lookup"><span data-stu-id="707ed-111">Type</span></span>|<span data-ttu-id="707ed-112">説明</span><span class="sxs-lookup"><span data-stu-id="707ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="707ed-113">path</span><span class="sxs-lookup"><span data-stu-id="707ed-113">path</span></span>|<span data-ttu-id="707ed-114">String</span><span class="sxs-lookup"><span data-stu-id="707ed-114">String</span></span>|<span data-ttu-id="707ed-115">Win32 基幹業務 (LoB) アプリケーションを検出するためにファイルまたはフォルダーのパス</span><span class="sxs-lookup"><span data-stu-id="707ed-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="707ed-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="707ed-116">fileOrFolderName</span></span>|<span data-ttu-id="707ed-117">String</span><span class="sxs-lookup"><span data-stu-id="707ed-117">String</span></span>|<span data-ttu-id="707ed-118">Win32 基幹業務 (LoB) アプリケーションを検出するためにファイルまたはフォルダーの名前</span><span class="sxs-lookup"><span data-stu-id="707ed-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="707ed-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="707ed-119">check32BitOn64System</span></span>|<span data-ttu-id="707ed-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="707ed-120">Boolean</span></span>|<span data-ttu-id="707ed-121">このファイルまたはフォルダーは、64 ビット システムで 32 ビット アプリケーションをチェックするかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="707ed-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="707ed-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="707ed-122">detectionType</span></span>|[<span data-ttu-id="707ed-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="707ed-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="707ed-124">ファイル システムの検出の種類。</span><span class="sxs-lookup"><span data-stu-id="707ed-124">The file system detection type.</span></span> <span data-ttu-id="707ed-125">使用可能な値: `notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`。</span><span class="sxs-lookup"><span data-stu-id="707ed-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="707ed-126">operator</span><span class="sxs-lookup"><span data-stu-id="707ed-126">operator</span></span>|[<span data-ttu-id="707ed-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="707ed-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="707ed-128">ファイルまたは fodler を検出するための演算子です。</span><span class="sxs-lookup"><span data-stu-id="707ed-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="707ed-129">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="707ed-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="707ed-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="707ed-130">detectionValue</span></span>|<span data-ttu-id="707ed-131">String</span><span class="sxs-lookup"><span data-stu-id="707ed-131">String</span></span>|<span data-ttu-id="707ed-132">ファイルまたはフォルダーの検出値</span><span class="sxs-lookup"><span data-stu-id="707ed-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="707ed-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="707ed-133">Relationships</span></span>
<span data-ttu-id="707ed-134">なし</span><span class="sxs-lookup"><span data-stu-id="707ed-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="707ed-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="707ed-135">JSON Representation</span></span>
<span data-ttu-id="707ed-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="707ed-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




