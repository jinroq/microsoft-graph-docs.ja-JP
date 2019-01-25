---
title: 'Microsoft グラフ API を使用して、ローマのプロジェクトを操作するには '
description: 'ローマのプロジェクトは、アプリケーション開発者は、デバイス間の優れたエクスペリエンスを構築できるプラットフォームを構築するのにはマイクロソフトの方針です。 ローマのプロジェクトは、同じ Microsoft を使用してユーザーがサインイン アカウントの機能、またはアカウントの学校とは、さまざまなサービスとクライアントのエンドポイントを接続する別の機能を有効にします。 これにより、デバイスではなく、ユーザーの作業の中心は、デバイス間およびプラットフォーム間でのエクスペリエンスを実装することができます。 '
localization_priority: Normal
ms.openlocfilehash: 57c5189f3caf64ec048d000d5e9108811bd88145
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509694"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="78626-105">Microsoft グラフ API を使用して、ローマのプロジェクトを操作するには</span><span class="sxs-lookup"><span data-stu-id="78626-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78626-106">[ローマのプロジェクト](https://developer.microsoft.com/en-us/windows/project-rome)は、アプリケーション開発者は、デバイス間の優れたエクスペリエンスを構築できるプラットフォームを構築するのにはマイクロソフトの方針です。</span><span class="sxs-lookup"><span data-stu-id="78626-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="78626-107">ローマのプロジェクトは、同じ Microsoft を使用してユーザーがサインイン アカウントの機能、またはアカウントの学校とは、さまざまなサービスとクライアントのエンドポイントを接続する別の機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="78626-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="78626-108">これにより、デバイスではなく、ユーザーの作業の中心は、デバイス間およびプラットフォーム間でのエクスペリエンスを実装することができます。</span><span class="sxs-lookup"><span data-stu-id="78626-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="78626-109">3 つの主要なローマのプロジェクト機能は、デバイス間のすばらしい経験を有効にするための Microsoft Graph では公開: 活動、デバイス、および通知します。</span><span class="sxs-lookup"><span data-stu-id="78626-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="78626-110">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="78626-110">Activities</span></span>

<span data-ttu-id="78626-111">Graph での活動、アプリを使用してドライブのユーザーの活動をデバイスやプラットフォーム間で、できます。</span><span class="sxs-lookup"><span data-stu-id="78626-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="78626-112">活動は、ユーザーの契約のユニットであるため、3 つのコンポーネントで構成されています。</span><span class="sxs-lookup"><span data-stu-id="78626-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="78626-113">緊密なリンク</span><span class="sxs-lookup"><span data-stu-id="78626-113">A deep link</span></span>
- <span data-ttu-id="78626-114">視覚的に表現</span><span class="sxs-lookup"><span data-stu-id="78626-114">A visual representation</span></span>
- <span data-ttu-id="78626-115">活動の内容を説明するコンテンツのメタデータを使用して、[https://schema.org/](https://schema.org/)のボキャブラリを共有</span><span class="sxs-lookup"><span data-stu-id="78626-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="78626-116">アプリケーションによってセッションが作成されると、ユーザーの活動の期間を反映するようにアクティビティを履歴項目が追加されます。</span><span class="sxs-lookup"><span data-stu-id="78626-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="78626-117">ユーザーは、アクティビティに reengages、たびに、新しい履歴項目がユーザーの活動を見越計上するアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="78626-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="78626-118">アプリケーションは、ユーザーのアクティビティ オブジェクトを公開して、ときにオブジェクトが表示されますいくつかの新しい UI の外観になります。たとえば、Cortana の通知をクリックします。</span><span class="sxs-lookup"><span data-stu-id="78626-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="78626-119">アクティビティ オブジェクトでは、豊富なメタデータを (適切なコンテキストで表示するアクティビティを許可する) と ([アダプティブ ・ カード](https://adaptivecards.io/)のマークアップを使用して)、豊富なビジュアルの両方を指定できます。</span><span class="sxs-lookup"><span data-stu-id="78626-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="78626-120">作成し、ユーザーのアクティビティを取得するのには次の Microsoft グラフ Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="78626-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="78626-121">活動の作成または</span><span class="sxs-lookup"><span data-stu-id="78626-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="78626-122">アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="78626-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="78626-123">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="78626-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="78626-124">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="78626-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="78626-125">履歴項目を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="78626-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="78626-126">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="78626-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="78626-127">デバイス</span><span class="sxs-lookup"><span data-stu-id="78626-127">Devices</span></span>

<span data-ttu-id="78626-128">Microsoft Graph では、プロジェクト ローマの Api を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="78626-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="78626-129">検出し、ユーザーのデバイスへの接続</span><span class="sxs-lookup"><span data-stu-id="78626-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="78626-130">これらのデバイスにアプリケーションをリモートで起動します。</span><span class="sxs-lookup"><span data-stu-id="78626-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="78626-131">それらのデバイスのアプリケーションにメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="78626-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="78626-132">これらの api では、1 つのデバイスを越える豊富なエクスペリエンスを作成するアプリケーションを構築できます。</span><span class="sxs-lookup"><span data-stu-id="78626-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="78626-133">たとえば、大きな画面で起動するアプリケーションを拡張できます。</span><span class="sxs-lookup"><span data-stu-id="78626-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="78626-134">または別のユーザーのデバイスのアプリのコンパニオンの経験を作成できます。</span><span class="sxs-lookup"><span data-stu-id="78626-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="78626-135">他の Windows デバイスと通信するために、次の Microsoft グラフ Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="78626-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="78626-136">ユーザーのデバイスを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="78626-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="78626-137">デバイスにコマンドを送信します。</span><span class="sxs-lookup"><span data-stu-id="78626-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="78626-138">コマンドのステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="78626-138">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="notifications"></a><span data-ttu-id="78626-139">通知</span><span class="sxs-lookup"><span data-stu-id="78626-139">Notifications</span></span>

<span data-ttu-id="78626-140">Graph で通知 Api を使用するには上に同じユーザーが署名されている複数のエンドポイント経由で通知を配布します。</span><span class="sxs-lookup"><span data-stu-id="78626-140">You can use the notifications APIs in Microsoft Graph to deliver notifications across multiple endpoints that the same user is signed in on.</span></span> <span data-ttu-id="78626-141">デバイス アドレスとチャネルを心配するのではなく通知を転記するときは、ユーザーを直接対象できます。</span><span class="sxs-lookup"><span data-stu-id="78626-141">You can target a user directly when posting notifications instead of worrying about device addresses/channels.</span></span> <span data-ttu-id="78626-142">この方法では、デバイスを中心とした方法ではなく、人間を中心とした、右の通知シナリオを設計することに集中できます。</span><span class="sxs-lookup"><span data-stu-id="78626-142">This way, you can focus on designing the right notification scenarios in a human-centric, rather than a device-centric way.</span></span> 

<span data-ttu-id="78626-143">通知の生データ、または直接視覚的に通知を発行できます。</span><span class="sxs-lookup"><span data-stu-id="78626-143">You can publish a raw data notification or a direct visual notification.</span></span> <span data-ttu-id="78626-144">生データの通知が配信されると、デバイスのエンドポイントを受信し、通知を管理する[クライアント SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph の通知、Windows SDK のプロジェクト ローマの SDK の iOS および Android) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="78626-144">When a raw data notification is delivered to a device endpoint, you can then use the [client SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph notifications SDK for Windows, Project Rome SDK for iOS and Android) to receive and manage notifications.</span></span> <span data-ttu-id="78626-145">デバイスのエンドポイントに直接視覚的に通知を配信すると、プラットフォーム固有のネイティブの通知をユーザーに表示します。</span><span class="sxs-lookup"><span data-stu-id="78626-145">When a direct visual notification is delivered to a device endpoint, it shows the platform-specific native notification to the user.</span></span> 

<span data-ttu-id="78626-146">詳細については、[作成し通知の送信](../api/projectrome-notification-post.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78626-146">For details, see [Create and send a notification](../api/projectrome-notification-post.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/project-rome-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
