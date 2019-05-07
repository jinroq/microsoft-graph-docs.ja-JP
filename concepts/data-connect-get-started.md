---
title: Microsoft Graph データ接続を始める
description: 'Microsoft Graph データ接続を使用する前に、Office 365 管理者は 2 つの処理を行う必要があります。どちらも、管理者が Privileged Access Management (PAM) を通じてデータ移動を制御する機能を有効にします。 '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 8372653d8904ba247975a649e6709b2206a4d6d3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33599787"
---
# <a name="get-started-with-microsoft-graph-data-connect"></a><span data-ttu-id="19c12-103">Microsoft Graph データ接続を始める</span><span class="sxs-lookup"><span data-stu-id="19c12-103">Get started with Microsoft Graph data connect (preview)</span></span>

<span data-ttu-id="19c12-104">Microsoft Graph データ接続を使用する前に、Office 365 管理者は 2 つの処理を行う必要があります。どちらも、管理者が Privileged Access Management (PAM) を通じてデータ移動を制御する機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="19c12-104">Before you can use Microsoft Graph data connect, an Office 365 administrator must take two actions, both of which enable the ability for the admin to control data movement through Privileged Access Management (PAM).</span></span> 

1. <span data-ttu-id="19c12-105">Microsoft 365 管理ポータルの **[サービスとアドイン]** ページを通じて、Microsoft Graph データ接続にオプトインすることに同意します。</span><span class="sxs-lookup"><span data-stu-id="19c12-105">Give consent to opt in to Microsoft Graph data connect through the Microsoft 365 Admin Portal, on the **Services & add-ins** page.</span></span> <span data-ttu-id="19c12-106">これにより、Microsoft Azure へのデータ移動要求が許可されます (つまり、データのフル コントロール権は保持されたまま、Azure リソースからのアクセスが許可されます)。</span><span class="sxs-lookup"><span data-stu-id="19c12-106">This will allow data movement requests to Microsoft Azure (that is, keep full control over the data, but allow Azure resources to access it).</span></span> <span data-ttu-id="19c12-107">特定のパイプラインに対する承認が後で行われないかぎり、データは転送されません。</span><span class="sxs-lookup"><span data-stu-id="19c12-107">No data is transferred unless approval for a specific pipeline is provided later.</span></span>
2. <span data-ttu-id="19c12-108">Office 365 サブスクリプションの承認者グループを設定します。</span><span class="sxs-lookup"><span data-stu-id="19c12-108">Set an approver group within the Office 365 subscription.</span></span> <span data-ttu-id="19c12-109">承認者グループが空でないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="19c12-109">Make sure that the approver group is not empty.</span></span> <span data-ttu-id="19c12-110">グループ内のユーザーのみが、データ移動要求を承認できます。</span><span class="sxs-lookup"><span data-stu-id="19c12-110">Only the users in the group can approve data movement requests.</span></span>

## <a name="next-steps"></a><span data-ttu-id="19c12-111">次の手順</span><span class="sxs-lookup"><span data-stu-id="19c12-111">Next steps</span></span>

<span data-ttu-id="19c12-112">おめでとうございます。</span><span class="sxs-lookup"><span data-stu-id="19c12-112">Congratulations!</span></span> <span data-ttu-id="19c12-113">Azure のツールを使用してインテリジェントなアプリケーションの構築を開始する準備が整いました。</span><span class="sxs-lookup"><span data-stu-id="19c12-113">You're now ready to start building intelligent applications with Azure tooling.</span></span> <span data-ttu-id="19c12-114">手順の詳細については、[Microsoft Graph データ接続のトレーニング モジュール](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19c12-114">For detailed step-by-step instructions, see the [Microsoft Graph data connect training module](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span></span> <span data-ttu-id="19c12-115">Microsoft Graph データ接続の機能の詳細については、[データセット、区域、およびシンク](/concepts/data-connect-datasets.md) または、データ接続がサポートする [ユーザー選択とフィルター処理](/concepts/data-connect-filtering.md)を参照してください。 </span><span class="sxs-lookup"><span data-stu-id="19c12-115">For more information about the capabilities that Microsoft Graph data connect provides, see [datasets, regions, and sinks](/concepts/data-connect-datasets.md) or [user selection and filtering](/concepts/data-connect-filtering.md) that data connect supports.</span></span>
