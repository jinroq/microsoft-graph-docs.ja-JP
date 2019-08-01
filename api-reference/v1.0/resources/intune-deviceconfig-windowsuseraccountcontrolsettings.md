---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9d97f1d8caa7e8159f94e235c571441a443b24e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027560"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="975a1-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="975a1-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="975a1-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="975a1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="975a1-105">Windows ユーザーアカウント制御設定に指定できる値。</span><span class="sxs-lookup"><span data-stu-id="975a1-105">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="975a1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="975a1-106">Members</span></span>
|<span data-ttu-id="975a1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="975a1-107">Member</span></span>|<span data-ttu-id="975a1-108">値</span><span class="sxs-lookup"><span data-stu-id="975a1-108">Value</span></span>|<span data-ttu-id="975a1-109">説明</span><span class="sxs-lookup"><span data-stu-id="975a1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="975a1-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="975a1-110">userDefined</span></span>|<span data-ttu-id="975a1-111">.0</span><span class="sxs-lookup"><span data-stu-id="975a1-111">0</span></span>|<span data-ttu-id="975a1-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="975a1-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="975a1-113">常に通知</span><span class="sxs-lookup"><span data-stu-id="975a1-113">alwaysNotify</span></span>|<span data-ttu-id="975a1-114">1-d</span><span class="sxs-lookup"><span data-stu-id="975a1-114">1</span></span>|<span data-ttu-id="975a1-115">常に通知します。</span><span class="sxs-lookup"><span data-stu-id="975a1-115">Always notify.</span></span>|
|<span data-ttu-id="975a1-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="975a1-116">notifyOnAppChanges</span></span>|<span data-ttu-id="975a1-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="975a1-117">2</span></span>|<span data-ttu-id="975a1-118">アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="975a1-118">Notify on app changes.</span></span>|
|<span data-ttu-id="975a1-119">Notifyonappのすべての非追加暗転</span><span class="sxs-lookup"><span data-stu-id="975a1-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="975a1-120">1/3</span><span class="sxs-lookup"><span data-stu-id="975a1-120">3</span></span>|<span data-ttu-id="975a1-121">デスクトップを暗転せずに、アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="975a1-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="975a1-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="975a1-122">neverNotify</span></span>|<span data-ttu-id="975a1-123">2/4</span><span class="sxs-lookup"><span data-stu-id="975a1-123">4</span></span>|<span data-ttu-id="975a1-124">通知しません。</span><span class="sxs-lookup"><span data-stu-id="975a1-124">Never notify.</span></span>|



