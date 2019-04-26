---
title: Microsoft Graph のクロスデバイス エクスペリエンス
description: '複数デバイス時代のユーザーは、複数のプラットフォームやフォーム ファクターのデバイスを使いこなしています。朝のニュースをタブレットで読み、通勤電車の中では携帯電話でメールをチェックし、仕事場ではデスクトップ PC を使います。 夜になると、ホーム メディア コンソールで映画を見た後、スマート スピーカーでその日のニュースを確認します。 平均的なユーザーは、一日の中で複数のデバイスやプラットフォームをあれこれ使い分けています。 '
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 85d48d07f06d189f30c8eba9f7f0876353b3ff25
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570279"
---
# <a name="cross-device-experiences-in-microsoft-graph"></a>Microsoft Graph のクロスデバイス エクスペリエンス

複数デバイス時代のユーザーは、複数のプラットフォームやフォーム ファクターのデバイスを使いこなしています。朝のニュースをタブレットで読み、通勤電車の中では携帯電話でメールをチェックし、仕事場ではデスクトップ PC を使います。 夜になると、ホーム メディア コンソールで映画を見た後、スマート スピーカーでその日のニュースを確認します。 平均的なユーザーは、一日の中で複数のデバイスやプラットフォームをあれこれ使い分けています。 

以前なら、消費者は、フォーム ファクターに応じてそれぞれ独自の振る舞いをしていました。 しかし今、マルチデバイス時代の消費者は、さまざまなデバイスを全部使いこなして作業を行っています。 日常的な作業 (家で家族と共にするものであれ、仕事で同僚と共にするものであれ) は、本質的にデバイス中心というよりも**人中心**の作業です。 消費者は、出所が何であれ、何かしら画面というものを使用したいと考えています。 実際のところは、デバイスが壁となっていることが多く、デバイスの違いを越えて同じことをしようとすると、自分宛にメールを送ったり USB スティックを使ったりすることが必要になります。 複数のデバイスの間を行き来するのは、消費者にとってストレスとなり、重要な作業の場合、作業の最中にコンテキストを切り替えることは損失となります。 開発者にとっても、このことは挑戦となります。というのは、ユーザーがアプリを使う際にストレスを感じると、アプリの使用率が下がることになるからです。

Microsoft では、複数デバイス間での統一的作業を可能にするエクスペリエンスを生み出すプラットフォームを構築しています。これは、ユーザーに付いて移動する**人中心**のシナリオを実現し、フォーム ファクターやプラットフォームによらず複数デバイスの壁をなくします。 Microsoft Graph は、Azure Active Directory および Office 365 のデータにアクセスするための単一の統一エンドポイントを提供します。 さらに、Microsoft Graph を活用すれば、顧客のアクティビティやデバイスにアクセスして、デバイスやプラットフォームの境界を越える人中心の豊かなエクスペリエンスが実現されます。 

## <a name="why-invest-in-cross-device-experiences"></a>クロスデバイス エクスペリエンスに投資する理由

### <a name="let-customers-pick-up-where-they-leave-off-with-the-activity-feed-api"></a>アクティビティ フィール API によりユーザーは直前まで作業していたところから再開可能 
アクティビティにより、アプリのユーザーが、プラットフォームやデバイスを越えてシームレスに移行しながら実行する固有のタスクをキャプチャする手段が提供されます。それにより、ユーザーが希望する画面からすぐに作業を再開できるようになります。 アクティビティ フィードを使用することにより、ユーザーにとって最も重要な作業に関する人中心のビューを作成することができ、それにより、Web、モバイル、PC の間で切り替える際のストレスが軽減されます。 

### <a name="build-rich-cross-device-experiences-by-using-the-device-relay-api"></a>デバイス リレー API 使用によるクロスデバイスの豊かなエクスペリエンスを構築 
デバイス リレー API は、Microsoft のさまざまなデバイス (PC、Windows Phone、Xbox、IoT、HoloLens など) に加えて、Android および iOS のデバイスを公開します。 それにより、ユーザーの複数デバイスの間の境界を完全に打ち破ることができます。 ユーザーの環境を利用し、単一デバイスの壁をリアルタイムで越える豊かなエクスペリエンスを作成するようなアプリを構築できます。 

### <a name="engage-users-with-human-centric-cross-device-notifications-preview"></a>人中心のクロスデバイス通知を使用してユーザーと連携する (プレビュー)

通知は、ユーザーに連絡したり、連携したりするための最も効果的かつ直接的な方法の 1 つです。 

Microsoft Graph 通知 API を使用すると、通知をデバイス中心ではなく人中心の方法で伝えることができます。 通知を送信する対象ユーザーを設定し、Microsoft Graph 通知フレームワークによって、そのユーザーがサインインしている各エンドポイントに通知を送信できます。 また、Microsoft Graph 通知 API ではクロスデバイス通知管理も簡単なので、複数のユーザーのデバイス間で通知を同期し、ユーザーにとっての冗長性や中断の量を低減できます。 

## <a name="api-reference"></a>API リファレンス
これらのサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 のクロスデバイス エクスペリエンス向け API](/graph/api/resources/project-rome-overview?view=graph-rest-1.0)
- [Microsoft Graph ベータ版のクロスデバイス エクスペリエンス向け API](/graph/api/resources/project-rome-overview?view=graph-rest-beta)


## <a name="next-steps"></a>次のステップ

- [Microsoft Graph API を使用してクロスデバイス エクスペリエンスを有効にする](/graph/api/resources/cross-device-reference-overview?view=graph-rest-1.0)
- [Microsoft Graph のアクティビティ フィード API の詳細情報を確認する](activity-feed-concept-overview.md)
- [Microsoft Graph のデバイス リレー API の詳細情報を確認する](device-relay-concept-overview.md)
- [Microsoft Graph の Microsoft Graph 通知 API の詳細情報を確認する](notifications-concept-overview.md)
