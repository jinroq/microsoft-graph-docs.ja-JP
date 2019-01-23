---
title: appLogUploadState 列挙型
description: AppLogUploadStatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 58dcc0d4a15370d6449772d917e8994f0eb9e7bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431666"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="4f2bf-103">appLogUploadState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4f2bf-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="4f2bf-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f2bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4f2bf-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f2bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f2bf-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4f2bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f2bf-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="4f2bf-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="4f2bf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f2bf-108">Members</span></span>
|<span data-ttu-id="4f2bf-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f2bf-109">Member</span></span>|<span data-ttu-id="4f2bf-110">値</span><span class="sxs-lookup"><span data-stu-id="4f2bf-110">Value</span></span>|<span data-ttu-id="4f2bf-111">説明</span><span class="sxs-lookup"><span data-stu-id="4f2bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f2bf-112">保留中</span><span class="sxs-lookup"><span data-stu-id="4f2bf-112">pending</span></span>|<span data-ttu-id="4f2bf-113">0</span><span class="sxs-lookup"><span data-stu-id="4f2bf-113">0</span></span>|<span data-ttu-id="4f2bf-114">要求が処理を待機しているかの処理</span><span class="sxs-lookup"><span data-stu-id="4f2bf-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="4f2bf-115">完了</span><span class="sxs-lookup"><span data-stu-id="4f2bf-115">completed</span></span>|<span data-ttu-id="4f2bf-116">1</span><span class="sxs-lookup"><span data-stu-id="4f2bf-116">1</span></span>|<span data-ttu-id="4f2bf-117">ダウンロードの Azure blob にアップロードされたファイルを使用して要求を完了するとします。</span><span class="sxs-lookup"><span data-stu-id="4f2bf-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="4f2bf-118">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="4f2bf-118">failed</span></span>|<span data-ttu-id="4f2bf-119">2</span><span class="sxs-lookup"><span data-stu-id="4f2bf-119">2</span></span>|<span data-ttu-id="4f2bf-120">要求は、処理し、エラー状態で終了しました。</span><span class="sxs-lookup"><span data-stu-id="4f2bf-120">Request finished processing and in error state.</span></span>|




