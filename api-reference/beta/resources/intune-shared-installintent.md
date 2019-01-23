---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 386214850534080e59c5c14786fdba69d45d31f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405451"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="ff1a9-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="ff1a9-103">installIntent enum type</span></span>

> <span data-ttu-id="ff1a9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff1a9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff1a9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff1a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff1a9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff1a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff1a9-107">管理者が選択したインストールの目的に使用できる値</span><span class="sxs-lookup"><span data-stu-id="ff1a9-107">Possible values for the install intent chosen by the admin.</span></span>

## <a name="members"></a><span data-ttu-id="ff1a9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ff1a9-108">Members</span></span>
|<span data-ttu-id="ff1a9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ff1a9-109">Member</span></span>|<span data-ttu-id="ff1a9-110">値</span><span class="sxs-lookup"><span data-stu-id="ff1a9-110">Value</span></span>|<span data-ttu-id="ff1a9-111">説明</span><span class="sxs-lookup"><span data-stu-id="ff1a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff1a9-112">使用可能</span><span class="sxs-lookup"><span data-stu-id="ff1a9-112">available</span></span>|<span data-ttu-id="ff1a9-113">0</span><span class="sxs-lookup"><span data-stu-id="ff1a9-113">0</span></span>|<span data-ttu-id="ff1a9-114">使用可能なインストールの目的です。</span><span class="sxs-lookup"><span data-stu-id="ff1a9-114">Available install intent.</span></span>|
|<span data-ttu-id="ff1a9-115">必須</span><span class="sxs-lookup"><span data-stu-id="ff1a9-115">required</span></span>|<span data-ttu-id="ff1a9-116">1</span><span class="sxs-lookup"><span data-stu-id="ff1a9-116">1</span></span>|<span data-ttu-id="ff1a9-117">目的のインストールが必要です。</span><span class="sxs-lookup"><span data-stu-id="ff1a9-117">Required install intent.</span></span>|
|<span data-ttu-id="ff1a9-118">アンインストール</span><span class="sxs-lookup"><span data-stu-id="ff1a9-118">uninstall</span></span>|<span data-ttu-id="ff1a9-119">2</span><span class="sxs-lookup"><span data-stu-id="ff1a9-119">2</span></span>|<span data-ttu-id="ff1a9-120">目的のインストールをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="ff1a9-120">Uninstall install intent.</span></span>|
|<span data-ttu-id="ff1a9-121">availableWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="ff1a9-121">availableWithoutEnrollment</span></span>|<span data-ttu-id="ff1a9-122">3</span><span class="sxs-lookup"><span data-stu-id="ff1a9-122">3</span></span>|<span data-ttu-id="ff1a9-123">インストールの目的を登録しなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="ff1a9-123">Available without enrollment install intent.</span></span>|




