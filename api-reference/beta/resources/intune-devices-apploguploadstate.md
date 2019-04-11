---
title: りんご oguの adstate 列挙型
description: りんご ogu/ロードアウト adstatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b59210e7a00fde1e62e1cbc056f0bd34625330e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792735"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="e7b5a-103">りんご oguの adstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="e7b5a-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="e7b5a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7b5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7b5a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7b5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7b5a-106">りんご ogu/ロードアウト adstatus</span><span class="sxs-lookup"><span data-stu-id="e7b5a-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="e7b5a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e7b5a-107">Members</span></span>
|<span data-ttu-id="e7b5a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e7b5a-108">Member</span></span>|<span data-ttu-id="e7b5a-109">値</span><span class="sxs-lookup"><span data-stu-id="e7b5a-109">Value</span></span>|<span data-ttu-id="e7b5a-110">説明</span><span class="sxs-lookup"><span data-stu-id="e7b5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7b5a-111">対する</span><span class="sxs-lookup"><span data-stu-id="e7b5a-111">pending</span></span>|<span data-ttu-id="e7b5a-112">.0</span><span class="sxs-lookup"><span data-stu-id="e7b5a-112">0</span></span>|<span data-ttu-id="e7b5a-113">要求が処理を待機しているか、または処理中です</span><span class="sxs-lookup"><span data-stu-id="e7b5a-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="e7b5a-114">せ</span><span class="sxs-lookup"><span data-stu-id="e7b5a-114">completed</span></span>|<span data-ttu-id="e7b5a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e7b5a-115">1</span></span>|<span data-ttu-id="e7b5a-116">要求は、ダウンロードのために Azure blob にアップロードされたファイルを使用して完了します。</span><span class="sxs-lookup"><span data-stu-id="e7b5a-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="e7b5a-117">フェール</span><span class="sxs-lookup"><span data-stu-id="e7b5a-117">failed</span></span>|<span data-ttu-id="e7b5a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e7b5a-118">2</span></span>|<span data-ttu-id="e7b5a-119">要求が処理を完了し、エラー状態になっています。</span><span class="sxs-lookup"><span data-stu-id="e7b5a-119">Request finished processing and in error state.</span></span>|





