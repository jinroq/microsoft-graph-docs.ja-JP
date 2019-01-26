---
title: OneDrive アクティビティ レポート
description: OneDrive アクティビティ レポートを使用すると、OneDrive 上のファイルの操作を参照して、OneDrive のすべてのライセンス ユーザーのアクティビティを取得できます。 これらのレポートでは、共有されているファイルの数を表示して、コラボレーションの進捗レベルを把握することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9771507e336ecf82b93eb2c12d22f45f47eb74fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572592"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="f8edf-104">OneDrive アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="f8edf-104">OneDrive activity reports</span></span>

<span data-ttu-id="f8edf-105">OneDrive アクティビティ レポートを使用すると、OneDrive 上のファイルの操作を参照して、OneDrive のすべてのライセンス ユーザーのアクティビティを取得できます。</span><span class="sxs-lookup"><span data-stu-id="f8edf-105">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="f8edf-106">これらのレポートでは、共有されているファイルの数を表示して、コラボレーションの進捗レベルを把握することができます。</span><span class="sxs-lookup"><span data-stu-id="f8edf-106">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="f8edf-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8edf-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="f8edf-108">レポート</span><span class="sxs-lookup"><span data-stu-id="f8edf-108">Reports</span></span>

| <span data-ttu-id="f8edf-109">関数</span><span class="sxs-lookup"><span data-stu-id="f8edf-109">Function</span></span>                                 | <span data-ttu-id="f8edf-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f8edf-110">Return Type</span></span> | <span data-ttu-id="f8edf-111">説明</span><span class="sxs-lookup"><span data-stu-id="f8edf-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="f8edf-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="f8edf-112">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="f8edf-113">Stream</span><span class="sxs-lookup"><span data-stu-id="f8edf-113">Stream</span></span>      | <span data-ttu-id="f8edf-114">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="f8edf-114">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="f8edf-115">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="f8edf-115">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="f8edf-116">Stream</span><span class="sxs-lookup"><span data-stu-id="f8edf-116">Stream</span></span>      | <span data-ttu-id="f8edf-117">アクティブな OneDrive ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="f8edf-117">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="f8edf-118">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="f8edf-118">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="f8edf-119">Stream</span><span class="sxs-lookup"><span data-stu-id="f8edf-119">Stream</span></span>      | <span data-ttu-id="f8edf-120">いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="f8edf-120">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

