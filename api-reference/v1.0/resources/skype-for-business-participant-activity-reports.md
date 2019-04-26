---
title: Skype for Business 参加者アクティビティ レポート
description: Skype for Business 参加者アクティビティ レポートを使用して、組織全体の参加者アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5cfb5412cb2be03dcd3463714346e5f23ca6a5cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565997"
---
# <a name="skype-for-business-participant-activity-reports"></a><span data-ttu-id="51faf-104">Skype for Business 参加者アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="51faf-104">Skype for Business participant activity reports</span></span>

<span data-ttu-id="51faf-105">Skype for Business 参加者アクティビティ レポートを使用して、組織全体の参加者アクティビティの詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="51faf-105">You can use the Skype for Business participant activity reports to get details on conferencing activity across your organization.</span></span> <span data-ttu-id="51faf-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="51faf-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="51faf-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の参加者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51faf-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="reports"></a><span data-ttu-id="51faf-108">レポート</span><span class="sxs-lookup"><span data-stu-id="51faf-108">Reports</span></span>

| <span data-ttu-id="51faf-109">関数</span><span class="sxs-lookup"><span data-stu-id="51faf-109">Function</span></span>                                 | <span data-ttu-id="51faf-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="51faf-110">Return Type</span></span> | <span data-ttu-id="51faf-111">説明</span><span class="sxs-lookup"><span data-stu-id="51faf-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="51faf-112">アクティビティの数を取得する</span><span class="sxs-lookup"><span data-stu-id="51faf-112">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | <span data-ttu-id="51faf-113">ストリーム</span><span class="sxs-lookup"><span data-stu-id="51faf-113">Stream</span></span>      | <span data-ttu-id="51faf-114">組織からユーザーが参加した会議セッションの数と種類ついて、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="51faf-114">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="51faf-115">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="51faf-115">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="51faf-116">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="51faf-116">Get user counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | <span data-ttu-id="51faf-117">Stream</span><span class="sxs-lookup"><span data-stu-id="51faf-117">Stream</span></span>      | <span data-ttu-id="51faf-118">組織からユーザーが参加したそれぞれ別個のユーザーの数と会議セッションの種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="51faf-118">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="51faf-119">会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。</span><span class="sxs-lookup"><span data-stu-id="51faf-119">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span> |
| [<span data-ttu-id="51faf-120">時間 (分) を取得する</span><span class="sxs-lookup"><span data-stu-id="51faf-120">Get minute counts</span></span>](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | <span data-ttu-id="51faf-121">Stream</span><span class="sxs-lookup"><span data-stu-id="51faf-121">Stream</span></span>      | <span data-ttu-id="51faf-122">組織からユーザーが参加した会議セッションの長さ (分) と種類について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="51faf-122">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="51faf-123">会議セッションの種類には、オーディオ/ビデオがあります。</span><span class="sxs-lookup"><span data-stu-id="51faf-123">Types of conference sessions include audio/video.</span></span> |
