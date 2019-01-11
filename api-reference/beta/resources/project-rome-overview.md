---
title: 'Microsoft グラフ API を使用して、ローマのプロジェクトを操作するには '
description: 'ローマのプロジェクトは、アプリケーション開発者は、デバイス間の優れたエクスペリエンスを構築できるプラットフォームを構築するのにはマイクロソフトの方針です。 ローマのプロジェクトは、同じ Microsoft を使用してユーザーがサインイン アカウントの機能、またはアカウントの学校とは、さまざまなサービスとクライアントのエンドポイントを接続する別の機能を有効にします。 これにより、デバイスではなく、ユーザーの作業の中心は、デバイス間およびプラットフォーム間でのエクスペリエンスを実装することができます。 '
localization_priority: Normal
ms.openlocfilehash: 9f3b923bff5bad93036a1784090c8ce00763650f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830003"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="ff35f-105">Microsoft グラフ API を使用して、ローマのプロジェクトを操作するには</span><span class="sxs-lookup"><span data-stu-id="ff35f-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

> <span data-ttu-id="ff35f-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff35f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff35f-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff35f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff35f-108">[ローマのプロジェクト](https://developer.microsoft.com/en-us/windows/project-rome)は、アプリケーション開発者は、デバイス間の優れたエクスペリエンスを構築できるプラットフォームを構築するのにはマイクロソフトの方針です。</span><span class="sxs-lookup"><span data-stu-id="ff35f-108">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="ff35f-109">ローマのプロジェクトは、同じ Microsoft を使用してユーザーがサインイン アカウントの機能、またはアカウントの学校とは、さまざまなサービスとクライアントのエンドポイントを接続する別の機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="ff35f-109">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="ff35f-110">これにより、デバイスではなく、ユーザーの作業の中心は、デバイス間およびプラットフォーム間でのエクスペリエンスを実装することができます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-110">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="ff35f-111">3 つの主要なローマのプロジェクト機能は、デバイス間のすばらしい経験を有効にするための Microsoft Graph では公開: 活動、デバイス、および通知します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-111">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="ff35f-112">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="ff35f-112">Activities</span></span>

<span data-ttu-id="ff35f-113">Graph での活動、アプリを使用してドライブのユーザーの活動をデバイスやプラットフォーム間で、できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-113">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="ff35f-114">活動は、ユーザーの契約のユニットであるため、3 つのコンポーネントで構成されています。</span><span class="sxs-lookup"><span data-stu-id="ff35f-114">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="ff35f-115">緊密なリンク</span><span class="sxs-lookup"><span data-stu-id="ff35f-115">A deep link</span></span>
- <span data-ttu-id="ff35f-116">視覚的に表現</span><span class="sxs-lookup"><span data-stu-id="ff35f-116">A visual representation</span></span>
- <span data-ttu-id="ff35f-117">活動の内容を説明するコンテンツのメタデータを使用して、[https://schema.org/](https://schema.org/)のボキャブラリを共有</span><span class="sxs-lookup"><span data-stu-id="ff35f-117">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="ff35f-118">アプリケーションによってセッションが作成されると、ユーザーの活動の期間を反映するようにアクティビティを履歴項目が追加されます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-118">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="ff35f-119">ユーザーは、アクティビティに reengages、たびに、新しい履歴項目がユーザーの活動を見越計上するアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-119">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="ff35f-120">アプリケーションは、ユーザーのアクティビティ オブジェクトを公開して、ときにオブジェクトが表示されますいくつかの新しい UI の外観になります。たとえば、Cortana の通知をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ff35f-120">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="ff35f-121">アクティビティ オブジェクトでは、豊富なメタデータを (適切なコンテキストで表示するアクティビティを許可する) と ([アダプティブ ・ カード](https://adaptivecards.io/)のマークアップを使用して)、豊富なビジュアルの両方を指定できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-121">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="ff35f-122">作成し、ユーザーのアクティビティを取得するのには次の Microsoft グラフ Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-122">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="ff35f-123">活動の作成または</span><span class="sxs-lookup"><span data-stu-id="ff35f-123">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="ff35f-124">アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-124">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="ff35f-125">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="ff35f-125">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="ff35f-126">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="ff35f-126">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="ff35f-127">履歴項目を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="ff35f-127">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="ff35f-128">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="ff35f-128">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="ff35f-129">デバイス</span><span class="sxs-lookup"><span data-stu-id="ff35f-129">Devices</span></span>

<span data-ttu-id="ff35f-130">Microsoft Graph では、プロジェクト ローマの Api を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-130">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="ff35f-131">検出し、ユーザーのデバイスへの接続</span><span class="sxs-lookup"><span data-stu-id="ff35f-131">Discover and connect to user's devices</span></span>
- <span data-ttu-id="ff35f-132">これらのデバイスにアプリケーションをリモートで起動します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-132">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="ff35f-133">それらのデバイスのアプリケーションにメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-133">Send messages to your apps on those devices</span></span>

<span data-ttu-id="ff35f-134">これらの api では、1 つのデバイスを越える豊富なエクスペリエンスを作成するアプリケーションを構築できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-134">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="ff35f-135">たとえば、大きな画面で起動するアプリケーションを拡張できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-135">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="ff35f-136">または別のユーザーのデバイスのアプリのコンパニオンの経験を作成できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-136">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="ff35f-137">他の Windows デバイスと通信するために、次の Microsoft グラフ Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-137">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="ff35f-138">ユーザーのデバイスを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-138">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="ff35f-139">デバイスにコマンドを送信します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-139">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="ff35f-140">コマンドのステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-140">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="notifications"></a><span data-ttu-id="ff35f-141">通知</span><span class="sxs-lookup"><span data-stu-id="ff35f-141">Notifications</span></span>

<span data-ttu-id="ff35f-142">Graph で通知 Api を使用するには上に同じユーザーが署名されている複数のエンドポイント経由で通知を配布します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-142">You can use the notifications APIs in Microsoft Graph to deliver notifications across multiple endpoints that the same user is signed in on.</span></span> <span data-ttu-id="ff35f-143">デバイス アドレスとチャネルを心配するのではなく通知を転記するときは、ユーザーを直接対象できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-143">You can target a user directly when posting notifications instead of worrying about device addresses/channels.</span></span> <span data-ttu-id="ff35f-144">この方法では、デバイスを中心とした方法ではなく、人間を中心とした、右の通知シナリオを設計することに集中できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-144">This way, you can focus on designing the right notification scenarios in a human-centric, rather than a device-centric way.</span></span> 

<span data-ttu-id="ff35f-145">通知の生データ、または直接視覚的に通知を発行できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-145">You can publish a raw data notification or a direct visual notification.</span></span> <span data-ttu-id="ff35f-146">生データの通知が配信されると、デバイスのエンドポイントを受信し、通知を管理する[クライアント SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph の通知、Windows SDK のプロジェクト ローマの SDK の iOS および Android) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ff35f-146">When a raw data notification is delivered to a device endpoint, you can then use the [client SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph notifications SDK for Windows, Project Rome SDK for iOS and Android) to receive and manage notifications.</span></span> <span data-ttu-id="ff35f-147">デバイスのエンドポイントに直接視覚的に通知を配信すると、プラットフォーム固有のネイティブの通知をユーザーに表示します。</span><span class="sxs-lookup"><span data-stu-id="ff35f-147">When a direct visual notification is delivered to a device endpoint, it shows the platform-specific native notification to the user.</span></span> 

<span data-ttu-id="ff35f-148">詳細については、[作成し通知の送信](../api/projectrome-notification-post.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff35f-148">For details, see [Create and send a notification](../api/projectrome-notification-post.md).</span></span>

