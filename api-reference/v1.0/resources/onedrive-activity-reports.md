---
title: OneDrive アクティビティ レポート
description: OneDrive アクティビティ レポートを使用すると、OneDrive 上のファイルの操作を参照して、OneDrive のすべてのライセンス ユーザーのアクティビティを取得できます。 これらのレポートでは、共有されているファイルの数を表示して、コラボレーションの進捗レベルを把握することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: e403d53df04ebf5b76cf695a80c2a03769293f24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035932"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="483eb-104">OneDrive アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="483eb-104">OneDrive activity reports</span></span>

<span data-ttu-id="483eb-105">OneDrive アクティビティ レポートを使用すると、OneDrive 上のファイルの操作を参照して、OneDrive のすべてのライセンス ユーザーのアクティビティを取得できます。</span><span class="sxs-lookup"><span data-stu-id="483eb-105">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="483eb-106">これらのレポートでは、共有されているファイルの数を表示して、コラボレーションの進捗レベルを把握することができます。</span><span class="sxs-lookup"><span data-stu-id="483eb-106">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="483eb-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="483eb-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="483eb-108">レポート</span><span class="sxs-lookup"><span data-stu-id="483eb-108">Reports</span></span>

| <span data-ttu-id="483eb-109">関数</span><span class="sxs-lookup"><span data-stu-id="483eb-109">Function</span></span>                                 | <span data-ttu-id="483eb-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="483eb-110">Return Type</span></span> | <span data-ttu-id="483eb-111">説明</span><span class="sxs-lookup"><span data-stu-id="483eb-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="483eb-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="483eb-112">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="483eb-113">ストリーム</span><span class="sxs-lookup"><span data-stu-id="483eb-113">Stream</span></span>      | <span data-ttu-id="483eb-114">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="483eb-114">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="483eb-115">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="483eb-115">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="483eb-116">Stream</span><span class="sxs-lookup"><span data-stu-id="483eb-116">Stream</span></span>      | <span data-ttu-id="483eb-117">アクティブな OneDrive ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="483eb-117">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="483eb-118">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="483eb-118">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="483eb-119">Stream</span><span class="sxs-lookup"><span data-stu-id="483eb-119">Stream</span></span>      | <span data-ttu-id="483eb-120">いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="483eb-120">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

