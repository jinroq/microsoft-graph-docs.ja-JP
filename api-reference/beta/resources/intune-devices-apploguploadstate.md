---
title: りんご Oguの Adstate 列挙型
description: りんご Ogu/ロードアウト Adstatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ebfbed2517143cb4574d75afad77f2f822e503cd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983380"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="688a7-103">りんご Oguの Adstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="688a7-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="688a7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="688a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="688a7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="688a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="688a7-106">りんご Ogu/ロードアウト Adstatus</span><span class="sxs-lookup"><span data-stu-id="688a7-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="688a7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="688a7-107">Members</span></span>
|<span data-ttu-id="688a7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="688a7-108">Member</span></span>|<span data-ttu-id="688a7-109">値</span><span class="sxs-lookup"><span data-stu-id="688a7-109">Value</span></span>|<span data-ttu-id="688a7-110">説明</span><span class="sxs-lookup"><span data-stu-id="688a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="688a7-111">対する</span><span class="sxs-lookup"><span data-stu-id="688a7-111">pending</span></span>|<span data-ttu-id="688a7-112">.0</span><span class="sxs-lookup"><span data-stu-id="688a7-112">0</span></span>|<span data-ttu-id="688a7-113">要求が処理を待機しているか、または処理中です</span><span class="sxs-lookup"><span data-stu-id="688a7-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="688a7-114">せ</span><span class="sxs-lookup"><span data-stu-id="688a7-114">completed</span></span>|<span data-ttu-id="688a7-115">1-d</span><span class="sxs-lookup"><span data-stu-id="688a7-115">1</span></span>|<span data-ttu-id="688a7-116">要求は、ダウンロードのために Azure blob にアップロードされたファイルを使用して完了します。</span><span class="sxs-lookup"><span data-stu-id="688a7-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="688a7-117">フェール</span><span class="sxs-lookup"><span data-stu-id="688a7-117">failed</span></span>|<span data-ttu-id="688a7-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="688a7-118">2</span></span>|<span data-ttu-id="688a7-119">要求が処理を完了し、エラー状態になっています。</span><span class="sxs-lookup"><span data-stu-id="688a7-119">Request finished processing and in error state.</span></span>|





