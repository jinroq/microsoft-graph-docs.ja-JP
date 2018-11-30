---
title: Microsoft グラフ API を使用して、ローマのプロジェクトを操作するには
description: プロジェクトのローマは、デバイス間を構築するマイクロソフトの方針が発生したプラットフォームです。 ローマのプロジェクトでは、ユーザーがクライアント デバイス上でサインインに使用する同じ Microsoft アカウントを使用して署名する場合のアプリケーションと対話するには、ローカルのクライアントまたはサービスのアプリケーションとリモート ・ ホスト上のサービスを有効にします。 デバイスではなく、ユーザーの作業の中心は、プログラムのデバイス間およびプラットフォーム間での経験をできます。
ms.openlocfilehash: ab703ff76d3da4ec1c6a8cd1189f3d85e57bac65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022308"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="a1b5d-105">Microsoft グラフ API を使用して、ローマのプロジェクトを操作するには</span><span class="sxs-lookup"><span data-stu-id="a1b5d-105">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="a1b5d-106">[プロジェクトのローマ](https://developer.microsoft.com/en-us/windows/project-rome)は、デバイス間を構築するマイクロソフトの方針が発生したプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="a1b5d-107">ローマのプロジェクトでは、ユーザーがクライアント デバイス上でサインインに使用する同じ Microsoft アカウントを使用して署名する場合のアプリケーションと対話するには、ローカルのクライアントまたはサービスのアプリケーションとリモート ・ ホスト上のサービスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-107">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="a1b5d-108">デバイスではなく、ユーザーの作業の中心は、プログラムのデバイス間およびプラットフォーム間での経験をできます。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-108">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="a1b5d-109">これらのエクスペリエンスを有効にする Microsoft Graph を使用して、重要なコンポーネントが公開される: 活動します。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-109">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="a1b5d-110">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="a1b5d-110">Activities</span></span>

<span data-ttu-id="a1b5d-111">Graph での活動、アプリを使用してドライブのユーザーの活動をデバイスやプラットフォーム間で、できます。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="a1b5d-112">活動は、ユーザーの契約のユニットであるため、3 つのコンポーネントで構成されています。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="a1b5d-113">緊密なリンク</span><span class="sxs-lookup"><span data-stu-id="a1b5d-113">A deep link</span></span>
- <span data-ttu-id="a1b5d-114">視覚的に表現</span><span class="sxs-lookup"><span data-stu-id="a1b5d-114">A visual representation</span></span>
- <span data-ttu-id="a1b5d-115">活動の内容を説明するコンテンツのメタデータを使用して、[https://schema.org/](https://schema.org/)のボキャブラリを共有</span><span class="sxs-lookup"><span data-stu-id="a1b5d-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="a1b5d-116">アプリケーションによってセッションが作成されると、ユーザーの活動の期間を反映するようにアクティビティを履歴項目が追加されます。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="a1b5d-117">ユーザーは、アクティビティに reengages、たびに、新しい履歴項目がユーザーの活動を見越計上するアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="a1b5d-118">アプリケーションは、ユーザーのアクティビティ オブジェクトを公開して、ときにオブジェクトが表示されますいくつかの新しい UI の外観になります。たとえば、Cortana の通知をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="a1b5d-119">アクティビティ オブジェクトでは、豊富なメタデータを (適切なコンテキストで表示するアクティビティを許可する) と ([アダプティブ ・ カード](https://adaptivecards.io/)のマークアップを使用して)、豊富なビジュアルの両方を指定できます。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="a1b5d-120">作成し、ユーザーのアクティビティを取得するのには次の Microsoft グラフ Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="a1b5d-121">活動の作成または</span><span class="sxs-lookup"><span data-stu-id="a1b5d-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="a1b5d-122">アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="a1b5d-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="a1b5d-123">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="a1b5d-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="a1b5d-124">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="a1b5d-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="a1b5d-125">履歴項目を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="a1b5d-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="a1b5d-126">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="a1b5d-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

