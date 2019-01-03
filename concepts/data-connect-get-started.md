---
title: Microsoft Graph データ接続の開始 (プレビュー)
description: 'Microsoft Graph データ接続を使用する前に、Office 365 管理者は 2 つの処理を行う必要があります。どちらも、管理者が Privileged Access Management (PAM) を通じてデータ移動を制御する機能を有効にします。 '
author: ajacks-msft
ms.openlocfilehash: 1cd8d5734b0fd8b48df8a49fe0a833583c21148d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312083"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a><span data-ttu-id="d6455-103">Microsoft Graph データ接続の開始 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="d6455-103">Get started with Microsoft Graph data connect (preview)</span></span>

<span data-ttu-id="d6455-104">Microsoft Graph データ接続を使用する前に、Office 365 管理者は 2 つの処理を行う必要があります。どちらも、管理者が Privileged Access Management (PAM) を通じてデータ移動を制御する機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="d6455-104">Before you can use Microsoft Graph data connect, an Office 365 administrator must take two actions, both of which enable the ability for the admin to control data movement through Privileged Access Management (PAM).</span></span> 

1. <span data-ttu-id="d6455-105">Microsoft 365 管理ポータルの **[サービスとアドイン]** ページを通じて、Microsoft Graph データ接続にオプトインすることに同意します。</span><span class="sxs-lookup"><span data-stu-id="d6455-105">Give consent to opt in to Microsoft Graph data connect through the Microsoft 365 Admin Portal, on the **Services & add-ins** page.</span></span> <span data-ttu-id="d6455-106">これにより、Microsoft Azure へのデータ移動要求が許可されます (つまり、データのフル コントロール権は保持されたまま、Azure リソースからのアクセスが許可されます)。</span><span class="sxs-lookup"><span data-stu-id="d6455-106">This will allow data movement requests to Microsoft Azure (that is, keep full control over the data, but allow Azure resources to access it).</span></span> <span data-ttu-id="d6455-107">特定のパイプラインに対する承認が後で行われないかぎり、データは転送されません。</span><span class="sxs-lookup"><span data-stu-id="d6455-107">No data is transferred unless approval for a specific pipeline is provided later.</span></span>
2. <span data-ttu-id="d6455-108">Office 365 サブスクリプションの承認者グループを設定します。</span><span class="sxs-lookup"><span data-stu-id="d6455-108">Set an approver group within the Office 365 subscription.</span></span> <span data-ttu-id="d6455-109">承認者グループが空でないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="d6455-109">Make sure that the approver group is not empty.</span></span> <span data-ttu-id="d6455-110">グループ内のユーザーのみが、データ移動要求を承認できます。</span><span class="sxs-lookup"><span data-stu-id="d6455-110">Only the users in the group can approve data movement requests.</span></span>

<span data-ttu-id="d6455-111">詳細なステップバイステップの手順については、[Microsoft Graph データ接続のトレーニング モジュール](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6455-111">For detailed step-by-step instructions, see the [Microsoft Graph data connect training module](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="d6455-112">次のステップ</span><span class="sxs-lookup"><span data-stu-id="d6455-112">Next steps</span></span>

<span data-ttu-id="d6455-113">おめでとうございます。</span><span class="sxs-lookup"><span data-stu-id="d6455-113">Congratulations!</span></span> <span data-ttu-id="d6455-114">Azure のツールを使用してインテリジェントなアプリケーションの構築を開始する準備が整いました。</span><span class="sxs-lookup"><span data-stu-id="d6455-114">You're now ready to start building intelligent applications with Azure tooling.</span></span> <span data-ttu-id="d6455-115">サンプル アプリケーションと追加のドキュメントについては、[Microsoft Graph データ接続の GitHub レポ](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6455-115">For a sample application and additional documentation, see the [Microsoft Graph data connect GitHub repo](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).</span></span> 