---
title: Microsoft Graph データ接続を使用するためのヒント
description: Microsoft Graph データ接続を活用するのに役立つヒントをご紹介します。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 7c887cf6a6407937c49d4e90b0c73800b13bee57
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629881"
---
# <a name="tips-for-using-microsoft-graph-data-connect"></a>Microsoft Graph データ接続を使用するためのヒント

Microsoft Graph データ接続を使用することにより、Microsoft Graph の膨大なデータセットへのマネージド アクセスを提供できるアプリケーションの開発が可能になります。 この記事では、データ接続機能を活用するのに役立つヒントをご紹介します。 Microsoft Graph データ接続の概要については、「[Microsoft Graph データ接続の概要](data-connect-concept-overview.md)」を参照してください。

## <a name="is-microsoft-graph-data-connect-right-for-you"></a>Microsoft Graph データ接続は適切な選択か

データ接続と Microsoft Graph API は、双方がアクセスする基になるデータは同じですが、アクセス方法は大きく異なります。 データ接続は、大量のデータを一括して抽出するように設計されています。これに対して、Microsoft Graph API は、個別のデータ セットにリアルタイムにアクセスするのにより適しています。 両者を組み合わせて使用するのが適切な場合もあります。 たとえば、去年のメール データをまず抽出する際にはデータ接続を使用し、次に、リアルタイムに作業を進めながらメールを分析する際に Microsoft Graph API を使用するといった方法が考えられます。 データ接続と Microsoft Graph API は、用途が異なる別なツールです。 実現したいシナリオに最適なアクセス方法はどちらかを検討することが大切です。

## <a name="expect-an-initial-overhead"></a>イニシャル オーバーヘッドを予測する

データ接続は大量のデータを一括して抽出するように設計されているため、データを抽出できるようになる前に、ある程度のオーバーヘッドが発生します。 このオーバーヘッドは約 45 分です。つまり、データ サイズに関わりなくすべてのパイプラインで、その程度の時間が最低必要になります。 大量のデータ処理の代償としてこれが無視できる場合もありますが、実現したいシナリオにとってその時間が許容できないものである場合は、Microsoft Graph API を活用するアプローチの方が望ましい可能性があります。

## <a name="data-must-stay-within-the-organizations-subscription"></a>データは組織のサブスクリプション内に保持する必要がある

データ接続パイプラインは、Azure サブスクリプション内で実行されるデータ統合サービスである Azure Data Factory によってオーケストレーションされます。 その Azure サブスクリプションは、[1 つのみの Office 365 テナントに関連付け](https://docs.microsoft.com/ja-JP/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)られています。 このため、データは、関連付けられている Azure サブスクリプションにまず渡される必要があります。 さらに最小化や集計を行うことにより、データは他でも利用できるようになります。

Office 365 データの抽出に他のユーザーが使用できるアプリを構築したい場合は、そのアプリを [Azure マネージド アプリケーション](https://docs.microsoft.com/ja-JP/azure/managed-applications/overview)としてパッケージ化し、Azure Marketplace に公開できます。 そうすることにより、ユーザーはそのアプリを自分の Azure サブスクリプションにデプロイでき、自分のテナントに含まれるデータにそのアプリでアクセスできるようになります。 

## <a name="use-of-service-principals"></a>サービス プリンシパルの使用

Data Factory パイプラインを作成する際に、Office 365 にリンクされたサービスに対して、サービス プリンシパルを提供することが必要になります。 Azure では、サービス プリンシパルは、アプリケーションまたはサービス (つまり、ユーザーではない) を表すセキュリティ ID です。 データ接続は、Office 365 データへの承認されたアクセスを取得する際に、その ID としてサービス プリンシパルを使用します。
他のユーザーが自分のテナントで使用できる Azure マネージド アプリケーションを作成する場合も、そのアプリが使用するサービス プリンシパルをアプリの発行元が提供します。 このサービス プリンシパルは、発行元のテナント内に置かれます。 ただし、アプリで他のサービス プリンシパルが必要になる場合は、インストールしたユーザーが自分のテナント内にサービス プリンシパルを作成します。 たとえば、Data Factory パイプラインが Azure のストレージ リソースにアクセスすることが必要になる場合があります。 ユーザーは、パイプラインが使用するストレージ アカウントへのアクセス許可を指定したサービス プリンシパルを作成します。

## <a name="check-for-pending-privileged-access-management-requests"></a>保留中の特権アクセス管理要求を確認する

管理者が特権アクセス管理 (PAM) 要求を許可してからでなければ、データ接続はデータをコピーできません。 PAM は、Office 365 でデータへのデータ パイプライン アクセスを承認するために使用されるメカニズムです。 初めてパイプラインをトリガーする際に、PAM は Office 365 管理者 (または指定された代理人) がそのアクセス要求を承認するまで待機します。 パイプラインの状態は "**処理中**" と表示されますが、次のスクリーンショットに示すように、基になるコピー アクティビティは、承認がなされるまで **ConsentPending** の状態になります。

![ConsentPending の状態であることを示すパイプライン実行状態ウィンドウのスクリーンショット](images/data-connect-tips.png)

開発中、特にパイプラインを変更した後は、パイプラインの実行が **ConsentPending** で停止しないことを確認なさるようにお勧めします。 たとえば、スキーマに別のフィールドを追加すると、次にパイプラインを実行する時に、承認を必要とする新しい PAM 要求が発行されます。 承認を待機しているパイプラインの処理をただ待っていては、時間が無駄になってしまいます。

## <a name="approve-pam-requests-via-office-365-admin-portal"></a>Office 365 管理ポータルから PAM 要求を承認する

データ接続の説明書には、PowerShell や PAM UX を使用して PAM 要求を承認する方法が説明されています。 PAM UX を使用して承認するには、[Office 365 管理ポータル](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/Settings/PrivilegedAccess)の PAM インターフェイスに移動します。 このポータルを使用すると、簡単でわかりやすい方法で PAM 要求を表示して、要求を承認、拒否、取り消すことができます。 ポータルへのリンクは、**[設定]** > **[サービスとアドイン]** > **[Microsoft Graph データ接続]** の順に選択すると、[Microsoft Graph データ接続のアドイン] にあります。

## <a name="use-a-second-user-to-approve-pam-requests"></a>PAM 要求を承認するため、第 2 のユーザーを使用する

パイプラインを実行して PAM 要求をトリガーする場合、そのパイプラインが使用するサービス プリンシパルを所有するユーザー アカウントに、その要求は関連付けられます。 このアカウントが、開発者が設定した承認者グループに属する場合でも、PAM 要求の承認にそのアカウントを使用することはできません。これは、自己承認が許可されていないためです。 実行しようとすると、PAM ポータルに "要求元と承認者が同じです。 自己承認は許可されていません" というエラー メッセージが表示されます。 開発向けに、要求を承認する管理者に加えて、第 2 のアカウントを作成できます。 提出者と承認者の双方に、アクティブな Exchange Online アカウントが必要です。

## <a name="deduplicate-emails-when-needed"></a>必要に応じて重複するメールを削除する

`Message` データセットからメールを抽出する際に、同じメールの JSON オブジェクトが複数存在することがよくあります。 このような重複は、メールが複数の宛先に送信された場合、各受信者のメールボックスにそのメールのコピーが存在することが原因です。 データセットは各メールボックスから抽出されるため、全ユーザーのコピーがすべて含まれることになります。 一部のシナリオではコピーをすべて保持する必要がありますが、そうでなければ、重複を削除できます。
エクスポートされた JSON オブジェクトの重複は、メッセージの `internetMessageId` に基づいて削除できます。`internetMessageId` が同じメッセージが 2 つあれば、それらは同一インスタンスの重複するコピーです。 重複は異なる BLOB に存在することもあるので、BLOB ごとに重複を削除するのではなく、すべての BLOB を対象に重複を削除する必要があります。

## <a name="use-puser-field-to-determine-the-relevant-user"></a>puser フィールドを使用して関連するユーザーを特定する

抽出したデータには、対応する Microsoft Graph API を使用する時点では存在しないメタ プロパティがいくつか含まれます。 特に `puser` フィールドは、データの抽出元ユーザーを特定するのに役立ちます。 同じメールのコピー 2 つが異なるメールボックスにあるシナリオでは、`puser` フィールドを使用することで、どちらのコピーがどのメールボックスから抽出されたかを特定できます。
`puser` フィールドは、`Manager` データセットなどのデータセットにも役立ちます。 エクスポートされた JSON にはマネージャーに関する情報が含まれますが、この情報が役立つのはそのマネージャーが誰のマネージャーであるかを知っている場合に限られます。 `puser` フィールドから、その JSON オブジェクトが一致するのは誰のマネージャーであるかを確認できます。

## <a name="next-steps"></a>次のステップ

機能に関するリクエストがあれば、[UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581) からお寄せください。 
