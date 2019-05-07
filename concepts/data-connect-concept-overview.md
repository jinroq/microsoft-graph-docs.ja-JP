---
title: Microsoft Graph データ接続の概要
description: Microsoft Graph データ接続が Office 365 データを Microsoft Azure へ移動することによって、ユーザーはデータの操作に最適な開発とホスティング ツールにアクセスできるようになります。
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 4f04a48119ecd4da282a0235d0f321aa769cba31
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33599801"
---
# <a name="overview-of-microsoft-graph-data-connect"></a>Microsoft Graph データ接続の概要
Microsoft Graph には、作業方法、コミュニケーション方法、共同作業方法、時間管理方法に関する情報を含む、従業員とその職場に関するリッチ データが含まれています。 Microsoft Graph データ接続が Microsoft Azure へ移動するデータを簡素化するツールを提供することで、ユーザーはデータの操作に最適な開発とホスティング ツールにアクセスできるようになります。 これにより、Microsoft Graph データに対する完全なコントロールを維持したまま、生産性を向上させる、革新的な業界固有のアプリケーションを活用することができます。 Microsoft は、お客様が期待する、より安全なコントロールを提供しています。

## <a name="why-use-microsoft-graph-data-connect"></a>Microsoft Graph データ接続を使用する理由
Office 365 管理者は、組織のデータを大量に移動し管理することに固有の課題について、慎重に考慮する必要があります。 Microsoft Graph データ接続は、データの新しいコントロール方法を管理者に提供するよう設計されています。データを使用して、データに基づく分析情報を作成するアプリを構築できます。 

### <a name="enable-granular-consent"></a>同意対象の細分化

Microsoft Graph の同意モデルでは、管理者またはユーザーは、特定の定義済みエンティティ セットへのアクセスを求めるアプリケーションの要求に対してのみ、許可または拒否することができます。 たとえば、Mail.Read への要求には、すべてのプロパティを持つ[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) インスタンス全体を含む、Outlook メールをサポートする固定のエンティティ セットに対する読み取りアクセス権が含まれます。 それに対して、Microsoft Graph データ接続の場合、同意対象の細分化が可能です。つまり、アプリケーションがあるエンティティ内の特定のプロパティに対するアクセスを要求したり、そのプロパティ内のデータをフィルター処理したりすることが可能になります。 管理者が Microsoft Graph データへのアクセスを明示的に承認しないかぎり、アクセスは許可されません。 要求では、要求するアクセスのレベルを指定し、データ ポリシーの適用、要求理由、要求データのスキーマを記述する必要があります。 結果として、アプリケーションはその機能で必要とするデータ以外は使用することができず、関連性のないコンテンツは除外されます。 たとえば、アプリはメールのメタデータをのみを使用し、本文と添付ファイルは除外します。 

### <a name="provide-data-governance"></a>データ ガバナンスの提供
Microsoft は、お客様のデータの状態に関する、Microsoft Graph と Azure 間の豊富で密接したコミュニケーションを促進しています。 Microsoft Graph データ接続を介してアプリケーションを構築する場合、準拠する予定の詳細なポリシーのセットを指定できます。 Office 365 管理者はこれらのポリシーを確認し、同意することができます。 この方法により、コンプライアンス管理のオーバーヘッドを最小限に抑えることができます。 同意がなされると、Microsoft はそのアプリケーションのポリシーへの準拠状況を監視します。 組織により設定されたポリシーにアプリケーションが違反している (または違反しようとしている) 場合、Microsoft はそのアプリケーションへのデータの提供を停止します。 

### <a name="get-access-to-data-at-scale"></a>大量のデータへのアクセス権の取得
リッチ アプリケーションでは、多くの場合は組織内の多数のユーザーが同時に、大量のデータに対してアクセスすることが必要となります。 従来のトランザクション データ モデルの場合、このようなデータ提供を実現するためには、複雑なインフラストラクチャを構築し、何千もの API 呼び出しを実行する必要があります。 Microsoft Graph データ接続の場合、Azure Data Factory を利用して、定期的に、いくつかの簡単な手順だけで、組織の Office 365 のデータをアプリケーションに提供できます。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

## <a name="next-steps"></a>次の手順
作業を開始するには、「[Microsoft Graph データ接続の開始](data-connect-get-started.md)」を参照してください。
