---
title: OneDrive アクティビティ レポート
description: OneDrive 上のファイルとの相互作用を参照して OneDrive を使用するライセンスのすべてのユーザーの利用状況を取得できます。 共有されるファイルの数を表示することによって起こっているのコラボレーションのレベルを理解することができます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8e02e93d2266f302fb3f90ab47fe4853e34adee5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947198"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="d8119-104">OneDrive アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="d8119-104">OneDrive activity reports</span></span>

> <span data-ttu-id="d8119-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d8119-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8119-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8119-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8119-107">OneDrive 上のファイルとの相互作用を参照して OneDrive を使用するライセンスのすべてのユーザーの利用状況を取得できます。</span><span class="sxs-lookup"><span data-stu-id="d8119-107">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="d8119-108">共有されるファイルの数を表示することによって起こっているのコラボレーションのレベルを理解することができます。</span><span class="sxs-lookup"><span data-stu-id="d8119-108">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="d8119-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8119-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="d8119-110">レポート</span><span class="sxs-lookup"><span data-stu-id="d8119-110">Reports</span></span>

| <span data-ttu-id="d8119-111">関数</span><span class="sxs-lookup"><span data-stu-id="d8119-111">Function</span></span>                                 | <span data-ttu-id="d8119-112">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8119-112">CSV return type</span></span> | <span data-ttu-id="d8119-113">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8119-113">JSON return type</span></span>                         | <span data-ttu-id="d8119-114">説明</span><span class="sxs-lookup"><span data-stu-id="d8119-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d8119-115">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="d8119-115">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="d8119-116">Stream</span><span class="sxs-lookup"><span data-stu-id="d8119-116">Stream</span></span>          | [<span data-ttu-id="d8119-117">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d8119-117">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="d8119-118">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="d8119-118">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="d8119-119">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="d8119-119">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="d8119-120">Stream</span><span class="sxs-lookup"><span data-stu-id="d8119-120">Stream</span></span>          | [<span data-ttu-id="d8119-121">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="d8119-121">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="d8119-122">アクティブな OneDrive ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="d8119-122">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="d8119-123">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="d8119-123">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="d8119-124">Stream</span><span class="sxs-lookup"><span data-stu-id="d8119-124">Stream</span></span>          | [<span data-ttu-id="d8119-125">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="d8119-125">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="d8119-126">いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="d8119-126">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
