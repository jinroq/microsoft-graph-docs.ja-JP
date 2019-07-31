---
title: Microsoft Intune での会社の使用条件-Microsoft Graph API
description: テナント組織の使用条件を定義する Intune エンドポイント (REST) の Microsoft Graph API を一覧表示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: a94e8179bd0064c7eb10f88551b7192f830cdcd4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011947"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="0a088-103">Microsoft Intune の会社の使用条件</span><span class="sxs-lookup"><span data-stu-id="0a088-103">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="0a088-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a088-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a088-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a088-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a088-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a088-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a088-107">Intune の使用条件をユーザー グループに展開して、登録、作業リソースへのアクセス、ポータル サイト アプリがデバイスやユーザーにどのように影響するかを説明することができます。</span><span class="sxs-lookup"><span data-stu-id="0a088-107">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="0a088-108">ポータル サイトを使用して自分の仕事に登録してアクセスするには、ユーザーはまず使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a088-108">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="0a088-109">さまざまな使用条件を含む複数のポリシーを作成して展開することができます。</span><span class="sxs-lookup"><span data-stu-id="0a088-109">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="0a088-110">同じ使用条件のバージョンを異なる言語で作成し、それぞれ適切なグループに展開することもできます。</span><span class="sxs-lookup"><span data-stu-id="0a088-110">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="0a088-111">次の Graph リソースを使用して、Intune での会社の使用条件を管理できます。</span><span class="sxs-lookup"><span data-stu-id="0a088-111">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="0a088-112">使用条件</span><span class="sxs-lookup"><span data-stu-id="0a088-112">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="0a088-113">使用条件の承認状態</span><span class="sxs-lookup"><span data-stu-id="0a088-113">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="0a088-114">使用条件の割り当て</span><span class="sxs-lookup"><span data-stu-id="0a088-114">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="0a088-115">条項および条件のグループの割り当て</span><span class="sxs-lookup"><span data-stu-id="0a088-115">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)
