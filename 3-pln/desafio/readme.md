# Análise dos Resultados do Speech Analyzer - Sentiment and opinion mining tryout

{
    "documents": [
        {
            "id": "id__1497",
            "sentiment": "mixed",
            "confidenceScores": {
                "positive": 0.74,
                "neutral": 0.01,
                "negative": 0.25
            },
            "sentences": [
                {
                    "sentiment": "positive",
                    "confidenceScores": {
                        "positive": 0.95,
                        "neutral": 0.04,
                        "negative": 0.01
                    },
                    "offset": 0,
                    "length": 40,
                    "text": "I bought a size S and it fit perfectly. ",
                    "targets": [],
                    "assessments": []
                },
                {
                    "sentiment": "negative",
                    "confidenceScores": {
                        "positive": 0,
                        "neutral": 0,
                        "negative": 0.99
                    },
                    "offset": 40,
                    "length": 84,
                    "text": "I found the zipper a little bit difficult to get up & down due to the side rushing. ",
                    "targets": [
                        {
                            "sentiment": "negative",
                            "confidenceScores": {
                                "positive": 0,
                                "negative": 1
                            },
                            "offset": 52,
                            "length": 6,
                            "text": "zipper",
                            "relations": [
                                {
                                    "relationType": "assessment",
                                    "ref": "#/documents/0/sentences/1/assessments/0"
                                }
                            ]
                        }
                    ],
                    "assessments": [
                        {
                            "sentiment": "negative",
                            "confidenceScores": {
                                "positive": 0,
                                "negative": 1
                            },
                            "offset": 72,
                            "length": 9,
                            "text": "difficult",
                            "isNegated": false
                        }
                    ]
                },
                {
                    "sentiment": "positive",
                    "confidenceScores": {
                        "positive": 0.99,
                        "neutral": 0,
                        "negative": 0
                    },
                    "offset": 124,
                    "length": 48,
                    "text": "The color and material are beautiful in person. ",
                    "targets": [
                        {
                            "sentiment": "positive",
                            "confidenceScores": {
                                "positive": 1,
                                "negative": 0
                            },
                            "offset": 128,
                            "length": 5,
                            "text": "color",
                            "relations": [
                                {
                                    "relationType": "assessment",
                                    "ref": "#/documents/0/sentences/2/assessments/0"
                                }
                            ]
                        },
                        {
                            "sentiment": "positive",
                            "confidenceScores": {
                                "positive": 1,
                                "negative": 0
                            },
                            "offset": 138,
                            "length": 8,
                            "text": "material",
                            "relations": [
                                {
                                    "relationType": "assessment",
                                    "ref": "#/documents/0/sentences/2/assessments/0"
                                }
                            ]
                        }
                    ],
                    "assessments": [
                        {
                            "sentiment": "positive",
                            "confidenceScores": {
                                "positive": 1,
                                "negative": 0
                            },
                            "offset": 151,
                            "length": 9,
                            "text": "beautiful",
                            "isNegated": false
                        }
                    ]
                },
                {
                    "sentiment": "positive",
                    "confidenceScores": {
                        "positive": 0.99,
                        "neutral": 0,
                        "negative": 0
                    },
                    "offset": 172,
                    "length": 22,
                    "text": "Amazingly comfortable!",
                    "targets": [],
                    "assessments": []
                }
            ]
        }
    ],
    "errors": []
}