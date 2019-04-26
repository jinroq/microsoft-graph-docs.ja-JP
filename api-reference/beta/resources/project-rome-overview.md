---
title: 'Microsoft Graph API を使用してプロジェクトローマを操作する '
description: 'プロジェクトローマは、アプリ開発者が強力なクロスデバイスエクスペリエンスを構築できるようにするプラットフォームを構築するための Microsoft イニシアティブです。 プロジェクトローマは、ユーザーが同じ Microsoft アカウントまたは職場または学校のアカウントでサインインしたときに、さまざまなサービスとクライアントエンドポイントを接続するさまざまな機能を有効にします。 これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスを実装できます。 '
localization_priority: Normal
ms.openlocfilehash: b247c434c90ff0517d012f23254a70c591cdafd4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344068"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="cd1c8-105">Microsoft Graph API を使用してプロジェクトローマを操作する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd1c8-106">[プロジェクトローマ](https://developer.microsoft.com/en-us/windows/project-rome)は、アプリ開発者が強力なクロスデバイスエクスペリエンスを構築できるようにするプラットフォームを構築するための Microsoft イニシアティブです。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="cd1c8-107">プロジェクトローマは、ユーザーが同じ Microsoft アカウントまたは職場または学校のアカウントでサインインしたときに、さまざまなサービスとクライアントエンドポイントを接続するさまざまな機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="cd1c8-108">これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスを実装できます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="cd1c8-109">Microsoft Graph では、主に3つの主要なプロジェクトローマ機能が提供されています。これにより、大量のクロスデバイスエクスペリエンスを有効にすることができます。アクティビティ、デバイス、および通知。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="cd1c8-110">活アクティビティ</span><span class="sxs-lookup"><span data-stu-id="cd1c8-110">Activities</span></span>

<span data-ttu-id="cd1c8-111">Microsoft Graph のアクティビティを使用すると、デバイスやプラットフォームを越えてユーザーがアプリを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="cd1c8-112">アクティビティはユーザー契約の単位であり、3つのコンポーネントで構成されます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="cd1c8-113">ディープリンク</span><span class="sxs-lookup"><span data-stu-id="cd1c8-113">A deep link</span></span>
- <span data-ttu-id="cd1c8-114">視覚的な表現</span><span class="sxs-lookup"><span data-stu-id="cd1c8-114">A visual representation</span></span>
- <span data-ttu-id="cd1c8-115">[https://schema.org/](https://schema.org/)共有ボキャブラリを使用して、アクティビティを記述するコンテンツメタデータ</span><span class="sxs-lookup"><span data-stu-id="cd1c8-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="cd1c8-116">アプリケーションによってセッションが作成されると、ユーザーの活動期間を反映するために履歴項目がアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="cd1c8-117">ユーザーがアクティビティを再実行するたびに、新しい履歴アイテムが、[見越計上] ユーザー契約のアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="cd1c8-118">アプリケーションがユーザーアクティビティオブジェクトを公開すると、そのオブジェクトが Windows の新しい UI サーフェスの一部に表示されます。たとえば、Cortana の通知とタイムラインです。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="cd1c8-119">アクティビティオブジェクトでは、リッチメタデータ (アクティビティを正しいコンテキストで表示できるようにする) とリッチビジュアル ([アダプティブカード](https://adaptivecards.io/)マークアップを使用) の両方を指定できます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="cd1c8-120">ユーザーアクティビティを作成および取得するには、次の Microsoft Graph api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="cd1c8-121">アクティビティを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="cd1c8-122">アクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="cd1c8-123">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="cd1c8-124">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="cd1c8-125">履歴項目を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="cd1c8-126">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="cd1c8-127">デバイス</span><span class="sxs-lookup"><span data-stu-id="cd1c8-127">Devices</span></span>

<span data-ttu-id="cd1c8-128">Microsoft Graph では、次のように Project ローマ api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="cd1c8-129">ユーザーのデバイスを検出して接続する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="cd1c8-130">これらのデバイスでアプリをリモートで起動する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="cd1c8-131">これらのデバイス上のアプリにメッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="cd1c8-132">これらの api を使用して、単一のデバイスを超えする豊富なエクスペリエンスを作成するアプリを構築できます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="cd1c8-133">たとえば、大きい画面で起動するようにアプリを拡張することができます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="cd1c8-134">または、別のユーザーのデバイス上にあるアプリに対してコンパニオン環境を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="cd1c8-135">次の Microsoft Graph api を使用して、他の Windows デバイスと通信できます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="cd1c8-136">ユーザーのデバイスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="cd1c8-137">デバイスにコマンドを送信する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="cd1c8-138">コマンドの状態を取得する</span><span class="sxs-lookup"><span data-stu-id="cd1c8-138">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="notifications"></a><span data-ttu-id="cd1c8-139">通知</span><span class="sxs-lookup"><span data-stu-id="cd1c8-139">Notifications</span></span>

<span data-ttu-id="cd1c8-140">Microsoft Graph の通知 api を使用して、同じユーザーがサインインしている複数のエンドポイント間で通知を配信することができます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-140">You can use the notifications APIs in Microsoft Graph to deliver notifications across multiple endpoints that the same user is signed in on.</span></span> <span data-ttu-id="cd1c8-141">通知を投稿する際に、デバイスのアドレスやチャネルについて心配する代わりに、ユーザーを直接対象にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-141">You can target a user directly when posting notifications instead of worrying about device addresses/channels.</span></span> <span data-ttu-id="cd1c8-142">このようにすると、デバイス中心ではなく、人中心の通知シナリオの設計に集中できます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-142">This way, you can focus on designing the right notification scenarios in a human-centric, rather than a device-centric way.</span></span> 

<span data-ttu-id="cd1c8-143">生データ通知または直接的な視覚的通知を発行できます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-143">You can publish a raw data notification or a direct visual notification.</span></span> <span data-ttu-id="cd1c8-144">生データ通知がデバイスエンドポイントに配信されると、[クライアント SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph notification sdk for Windows、iOS 用 Project ローマ sdk) を使用して通知を受信し、管理することができます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-144">When a raw data notification is delivered to a device endpoint, you can then use the [client SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph notifications SDK for Windows, Project Rome SDK for iOS and Android) to receive and manage notifications.</span></span> <span data-ttu-id="cd1c8-145">ダイレクトビジュアル通知がデバイスエンドポイントに配信されるときに、プラットフォーム固有のネイティブ通知がユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-145">When a direct visual notification is delivered to a device endpoint, it shows the platform-specific native notification to the user.</span></span> 

<span data-ttu-id="cd1c8-146">詳細については、「[通知の作成と送信](../api/projectrome-notification-post.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd1c8-146">For details, see [Create and send a notification](../api/projectrome-notification-post.md).</span></span>

